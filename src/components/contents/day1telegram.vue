<template>
  <div>
    <DetailFormat>
      <template v-slot:title>
        認識 Telegram Bot
      </template>
      <template v-slot:subtitle>
        Day 1 16:30~17:30 (1hr)
      </template>
      <template v-slot:teacher>
        秉虎、鯉魚
      </template>
      <template v-slot:desc>
        <p>一隻魚跟一隻虎</p>
      </template>
      <template v-slot:content>
        <p>帶領學員大略認識 Telegram 各式功能，認識 Telegram 上面 bot 的各種互動形式及能做到的功能介紹</p>
      </template>
      <template v-slot:image>
        <img
          src
          alt
        >
      </template>
    </DetailFormat>
  </div>
</template>
<script>
import DetailFormat from './DetailFormat'
export default {
  components: {
    DetailFormat
  },
  data () {
    return {}
  }
}
</script>
