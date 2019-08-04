<template>
  <div>
    <DetailFormat>
      <template v-slot:title>資訊安全觀念入門</template>
      <template v-slot:subtitle>Day 2 13:30~14:30 (1hr)</template>
      <template v-slot:teacher>splitline</template>
      <template v-slot:desc>
        <p>魔化異能行者。</p>
      </template>
      <template v-slot:content>
        <p>黑魔法及黑魔法防禦術。</p>
        <p>本場講座將從「日常生活」以及「開發者」兩個面向來簡介資訊安全相關議題， 讓大家在這個資訊宇宙中能妥善應對各種黑魔法。同時亦會介紹相關社群與學 習資源，讓大家日後能繼續探索。</p>
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
