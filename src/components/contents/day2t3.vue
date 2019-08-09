<template>
  <div>
    <DetailFormat>
      <template v-slot:title>
        網路 / HTTP / RESTful 觀念及實做
      </template>
      <template v-slot:subtitle>
        Day 2 09:00 - 12:00 (3hr)
      </template>
      <template v-slot:teacher>
        Denny Huang
      </template>
      <template v-slot:desc>
        <p>
          SITCON 學生計算機年會共同發起人，2013 及 2014 年會總召，目前於雷亞遊戲（Rayark Inc.）擔任 Data Team Lead；
          在正規教育中特例獨行，妄想透過改善教育讓台灣更進步，崇尚開源精神，熱愛使用者界面 (UI) 以外的多種技術。
        </p>
      </template>
      <template v-slot:content>
        <p>
          課程錄影
          <a href="https://youtu.be/3r-Z2zcAhoI">https://youtu.be/3r-Z2zcAhoI</a><br />
          投影片連結
          <a href="https://denny.one/the-net/">https://denny.one/the-net/</a><br />
          共筆連結
          <a href="https://hackmd.io/@SITCON/camp2019-the-net">https://hackmd.io/@SITCON/camp2019-the-net</a>
        </p>
        <p>
          每天你在手機滑著 Instagram，又或是在電腦上打開瀏覽器逛著各種網頁，你是否有想過這些內容是如何呈現在你的眼前？
          聽到伺服器這個詞，你想到了什麼？架伺服器真的有這麼困難？到底伺服器要做什麼事情？
          這堂課程將帶你看透一切，過去對你來說或許是黑魔法的未知領域，在課程過後相信你對世界會有嶄新的看法！
        </p>
      </template>
      <template v-slot:image>
        <img
          src="../../assets/teachers/Denny.jpg"
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
