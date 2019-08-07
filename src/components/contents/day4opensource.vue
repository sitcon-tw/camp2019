<template>
  <div>
    <DetailFormat>
      <template v-slot:title>
        開源精神分享
      </template>
      <template v-slot:subtitle>
        Day 4 10:00~11:00 (1hr)
      </template>
      <template v-slot:teacher>
        小班
      </template>
      <template v-slot:desc>
        <p>小班，g0v 參與者，以文字工作參與 g0v 協作聚焦科技如何促進民主，支持資 訊透明和更開放的公民參與，未來想要成立一家公民科技公司。</p>
        <p>曾於 g0v 揪松 團擔任 g0v 公民科技獎助金專案經理，曾擔任 sense.tw 產品經理，開發議題政 策討論工具，目前在各地遊走。</p>
      </template>
      <template v-slot:content>
        <p>希望用輕鬆互動的方式向大家簡介開放原始碼運動(open source movement)，背後的精神、社群，大家為什麼要開源，國際和台灣的開源社 群發展，以及想要參與開源社群可以如何開始。</p>
      </template>
      <template v-slot:image>
        <img
          src="../../assets/teachers/小班 - Yun-Chen Chien.jpg"
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
