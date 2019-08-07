<template>
  <div>
    <DetailFormat>
      <template v-slot:title>
        社群闖關
      </template>
      <template v-slot:subtitle>
        Day 4 11:00~15:00 (4hr)
      </template>
      <template v-slot:teacher />
      <template v-slot:desc />
      <template v-slot:content>
        <p>社群闖關邀請到許多資訊相關社群前來擺攤，藉由互動遊戲、影片欣賞、專人介紹...等方式，讓學員認識所謂「社群」並對開源活動有初步了解。</p>
        <p>今年的夏令營我們請來 Mozilla 台灣社群、Fedora 臺灣社群、 Ubuntu-TW、HITCON GIRLS、Wikidata Taiwan、TDOHacker、 GDG Taipei、g0v.tw、PyCon Taiwan 等社群，敬請期待今年的活動。</p>
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
