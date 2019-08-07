<template>
  <div>
    <DetailFormat>
      <template v-slot:title>
        視界咖啡館
      </template>
      <template v-slot:subtitle>
        Day 4 15:00~17:30 (2.5hr)
      </template>
      <template v-slot:teacher />
      <template v-slot:desc />
      <template v-slot:content>
        <p>視界咖啡館參考自世界咖啡館 (The World Café)，在本次夏令營中，我們邀請到各領域及社群前輩，將傳統座談會形式改以小組 討論的樣貌呈現，並與學員分享工作經驗、學習過程、面對困難 的解決方式或希望給予 SITCON 夏令營學員的建議，提出值得學 員思考、了解的觀點。</p>
        <p>期望透過縮短講師及學員間的距離，鼓勵學員踴躍提問、參與， 進而產生良好的雙向交流。</p>
        <h4>Ronny</h4>
        <hr class="coffee-underline">
        <p>雖然現在我是靠寫程式吃飯，但在我高中專注在資訊社團時，我爸曾教訓過我 「未來人人都會用電腦，你會電腦有什麼用?」要我減少社團多多念書。前幾 年跟朋友創業時一度因挫折壓力大到我去看心理醫生，與心理醫生聊了兩個月 後，發現過去家庭對我造成了多深的影響，有好的有壞的影響，我覺得我家庭 並不特別，因此我的故事或許也可能是大家的故事。</p>
        <span
          class="coffeedesc"
        >
          <img
            src="../../assets/teachers/Ronny_Wang.jpg"
            alt=""
          >
          g0v 零時政府長期參與者，程式設計師，喜歡做開放政府資料相關應用，做過 台灣公司關係圖、新聞小幫手、求職小幫手、開放政治獻金等專案(可參考 https://ronny.tw/data )，在行政院和一些部會擔任開放資料諮詢委員。2004 年 PTT 名人投票得過第 7 名，擔任 PTT 就可板板主時發明了推齊和怡君賭盤， 2020 年成為了立委擬參選人。</span>

        <h4>Birdman</h4>
        <hr class="coffee-underline">
        <p>資安新視野。</p>
        <span
          class="coffeedesc"
        >
          <img
            src="../../assets/teachers/birdman_fix.jpg"
            alt=""
          >
          中央大學、大同資工碩士，是台灣資安界有多次創業經驗的企業家，曾在 2014 年由美國 NASDAQ 上市的以色列資安公司所併購與肯定。專注資安科技研究 多年，以開發自動化分析系統，駭客活動分析，惡意程式分析、人工智慧演 算法為主要研究範疇，HITCON 台灣駭客協會顧問，頂尖駭客會議 Blackhat / DEFCON / HITCON 講師。</span>

        <h4>PCMan</h4>
        <hr class="coffee-underline">
        <p>分享一路上自學軟體開發，經營開源軟體專案，到進入業界工作的心得。</p>
        <span class="coffeedesc">
          <img
            src="../../assets/teachers/PCMan.jpg"
            alt=""
          >
          <ul>
            <li>Appier Inc. 資深軟體工程師</li>
            <li>台大資訊工程研究所畢業</li>
            <li>18 年軟體開發 ( 自學 )</li>
            <li>LXDE / LXQt 桌面環境</li>
            <li>新酷音輸入法 windows port</li>
            <li>IE Tab Firefox 外掛</li>
            <li>前台北榮總風濕免疫科醫師</li>
            <li>陽明大學醫學系畢業</li>
            <li>主要參與 open source 專案 :</li>
            <ul>
              <li>PIME 輸入法平台</li>
              <li>PCMan BBS client 全系列</li>
            </ul>
          </ul>
        </span>

        <h4>LJ</h4>
        <hr class="coffee-underline">
        <P>空氣污染是台灣近年來面對的重大議題，面對如此與健康息息相關的威脅，民眾最迫切需要的是獲取在地與即時的空氣品質資訊，以增加對周遭環境的認知， 進而能夠適時採取適當的作為防護作為。</P>
        <P>「PM2.5 微型感測」計畫(又稱「空氣盒子」計畫)，便是一個以此為出發點， 從個人到社群、從學術界到產業界、從民間到政府單位，並且從台灣到全世界的參與式群眾感測計畫，透過開放的精神，</P>
        <P>從設備硬體、軟體、感測資料到各 項服務，透過所有參與者的共創、共學，共同建立起全世界最大的微型空氣品質感測系統，並且利用收集到的資料，提供即時異常偵測、短期空品預報，以及最佳空品導航等各項創新的資訊服務。</P>
        <P>在這場分享中，我們將介紹這個計畫 的緣起與發展過程，以及在這個計畫背後驅動各項研發成果的資訊科技。</P>
        <span class="coffeedesc">
          <img
            src="../../assets/teachers/20161020 - Ling-Jyh Chen.jpg"
            alt=""
          >
          <P>陳伶志博士目前是中央研究院資訊科學所研究員，研究專長是物聯網、網路感測技術與行動無線網路。陳博士歷年的代表性作品包含玉山登山客搜救系統、大台北公車舒適度評量系統，以及 PM2.5 微型感測系統。</P>
          <P>其中，陳博士近期所專注研發的 PM2.5 微型感測系統，已成功在全球 48 個國家佈建超過 10,000 個 感測裝置，不但成為台灣民眾獲取即時 PM2.5 濃度資訊的最重要資訊來源，並且帶動微型空氣品質感測研究領域在軟硬體與即時資料分析等各項技術的發 展。</P>
          <P>陳博士目前除了持續推動 PM2.5 微型感測系統的佈建外，更積極進行跨界的合作，希望能結合微型空品感測技術，在更多環境相關的議題上做出貢獻。</P>
        </span>
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
<style lang="scss">
.coffeedesc {
  display: block;
  border-left: solid 2px white;
  padding: 0px 16px;
  margin-left: 16px;
  line-height: 1.3;
  margin-bottom: 60px;
}
.coffee-underline {
  margin-top: -30px;
}
</style>
