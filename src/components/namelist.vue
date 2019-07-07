<template>
  <div class="main">
    <h4>正取學員</h4>
    <div class="list">
      <template v-for="(name, i) in namelist.a">
        <span :key="i">{{markname(name)}}</span>
      </template>
    </div>
    <h4>備取學員</h4>
    <div class="list">
      <template v-for="(name, i) in namelist.b">
        <span :key="i">{{markname(name)}}</span>
      </template>
    </div>
  </div>
</template>
<script>
import namelist from "../assets/json/namelist.json";

export default {
  data() {
    return { namelist };
  },
  mounted() {},
  beforeDestroy() {},

  methods: {
    markname(name) {
      return name.replace("?", "○");
    }
  }
};
</script>

<style scoped lang="scss">
.list {
  display: flex;
  flex-wrap: wrap;
  span {
    min-width: 100px;
    width: 100% * 1/6;
    padding: 10px 16px;
    white-space: nowrap;
    box-sizing: border-box;
  }
  justify-content: center;
}
</style>
