<template>
  <div>
    <DetailFormat>
      <template v-slot:title>資訊視野拓展</template>
      <template v-slot:subtitle>Day 3 13:30~14:30 (1hr)</template>
      <template v-slot:teacher>Johnson Lin</template>
      <template v-slot:desc>
        <p>自 2011 年初投入獨立遊戲開發相關活動推廣，在同好與朋友協助下，定期舉辦聚會、Game Jam 等社群活動，現為 IGDShare 獨立遊戲開發者分享會資深雜工、IGDA Taiwan 聯絡人，以及台北遊戲開發者論壇(TGDF)共同發起人。</p>
      </template>
      <template v-slot:content>
        <p>現在是個遊戲開發上不用 Unity 就沒人權的年代，而且如果用了 Unity 而不知利用 Unity Asses Store，也同樣沒啥人權。但是遊戲開發需要觸及的面向廣闊， 很多時候也不是單純開發工具上的問題。</p>
        <p>這邊就讓完全沒使用過 Unity 的我來稍微整理一下，除了大家目前較熟悉的常見開發工具之外，在遊戲開發起步時， 還有哪些資源可以利用，以及台灣在地能多參加的活動。</p>
      </template>
      <template v-slot:image>
        <img src alt />
      </template>
    </DetailFormat>
  </div>
</template>
<script>
import DetailFormat from "./DetailFormat";
export default {
  components: {
    DetailFormat
  },
  data() {
    return {};
  }
};
</script>
