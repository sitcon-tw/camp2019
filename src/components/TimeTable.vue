<template>
  <div class="parent">
    <div id="TimeTable">
      <div class="big-version">
        <table class="table-big">
          <thead>
            <tr>
              <th class="time">
                7:00
              </th>
              <th
                v-for="head in heads"
                :key="head"
              >
                {{ head }}
              </th>
            </tr>
          </thead>
          <tbody>
            <tr
              v-for="index in indexes"
              :key="index"
            >
              <td class="time">
                {{ /*times[index] + ' ~ ' +*/ times[index + 1] }}
              </td>
              <template v-for="day in days">
                <td
                  v-if="getEvent(times[index], day) !== undefined"
                  :key="day"
                  :class="{
                    event:true,
                    clickable: getEvent(times[index], day).detail!=null
                  }"
                  :rowspan="calcRowspan(index, getEvent(times[index], day))"
                  @click="$emit('selected', getEvent(times[index], day).detail)"
                >
                  <h4>{{ getEvent(times[index], day).title }}</h4>
                  <h5>{{ getEvent(times[index], day).subTitle }}</h5>
                </td>
              </template>
            </tr>
            <tr>
              <td class="hidden">
                .
              </td>
            </tr>
          </tbody>
        </table>
      </div>

      <div
        v-for="(day, id) in events_byday"
        :key="id"
        class="small-version"
      >
        <h4>Day {{ id }}</h4>
        <table class="table-small">
          <template v-for="(event, eid) in day">
            <tr
              v-if="event.subTitle!=''"
              :key="eid"
              :class="{
                clickable: event.detail!=null
              }"
              @click="$emit('selected', event.detail)"
            >
              <td>{{ event.time.start }}~ {{ event.time.end }}</td>
              <td>{{ event.subTitle }}</td>
            </tr>
          </template>
        </table>
      </div>
    </div>
  </div>
</template>

<script>
import events from '../assets/json/events.json'
import groupBy from 'lodash.groupby'
import range from 'lodash.range'
// import uniq from 'lodash.uniq'

function timeToNumber (time) {
  let separated = time.split(':')
  return separated[0] * 60 + +separated[1]
}

events.sort((a, b) => {
  return timeToNumber(a.time.start) - timeToNumber(b.time.start)
})

export default {
  name: 'TimeTable',
  components: {},
  events: ['selected'],
  data () {
    return {
      start: '07:30',
      end: '22:00',
      heads: [
        'Day 1 (8/7)',
        'Day 2 (8/8)',
        'Day 3 (8/9)',
        'Day 4 (8/10)',
        'Day 5 (8/11)'
      ],
      days: ['1', '2', '3', '4', '5'],
      events: events,
      events_byday: groupBy(events, 'time.day')
    }
  },
  computed: {
    groups: function () {
      return groupBy(this.events, 'time.start')
    },
    times: function () {
      const result = []
      for (let i = 0; result[result.length - 1] !== this.end; i++) {
        let time =
          this.getTime(this.start).hour * 60 +
          this.getTime(this.start).min +
          i * 30
        let temp = {
          hour: Math.floor(time / 60),
          min: time % 60
        }
        result.push(`${temp.hour}:${temp.min.toString().padStart('2', '0')}`)
      }
      return result
    },
    indexes: function () {
      return range(0, this.times.length - 1)
    }
  },
  methods: {
    getTime (value) {
      const sp = value.split(':')
      return {
        hour: Number(sp[0]),
        min: Number(sp[1])
      }
    },
    getEvent (time, day) {
      // console.log(time, day);
      if (this.groups[time]) {
        return this.groups[time].find(element => element.time.day === day)
      } else return undefined
    },
    calcRowspan (index, event) {
      let start =
        this.getTime(event.time.start).hour * 60 +
        this.getTime(event.time.start).min
      let end =
        this.getTime(event.time.end).hour * 60 +
        this.getTime(event.time.end).min
      return Math.floor((end - start) / 30)
    }
  }
}
</script>

<style lang="sass" scoped>
#TimeTable
  overflow-x: auto
  overflow-y: hidden
table.table-big
  width: 100%
  min-width: 600px
  box-sizing: border-box
  border-collapse: separate
  background-color: rgba(0,0,0,0.5)
  th,td
    vertical-align: middle
    border: 1px solid #aaa

    h4,h5
      margin: 0
  .time
    height: 40px
    transform: translate(0,50%)
    border: none
    padding: 2px
  .event
    width: 140px
  .hidden
    opacity: 0
</style>

<style scoped lang="scss">
@import "../style/main.scss";

table.table-small {
  width: 100%;
  border-collapse: collapse;
  // border: solid 1px white;
  background-color: rgba(0, 0, 0, 0.5);

  td {
    padding: 8px;
    border-top: solid 1px gray;
  }
}
.small-version {
  display: none;
}
@include rwd-below(630px) {
  .small-version {
    display: block;
  }
  .big-version {
    display: none;
  }
}

.clickable{
  cursor: pointer;
  &:hover{
    background-color: rgba(255, 255, 255, .2);
  }
}
</style>
