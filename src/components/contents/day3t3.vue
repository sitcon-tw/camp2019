<template>
  <div>
    <DetailFormat>
      <template v-slot:title>
        package management、pip &amp; requests、handle json data
      </template>
      <template v-slot:subtitle>
        Day 3 09:00 - 12:00 (3hr)
      </template>
      <template v-slot:teacher>
        soyccan / 正康
      </template>
      <template v-slot:desc>
        <p>交通大學電資班大一，曾經在南一中資訊社當教學，現在是天文社的儀器長，是SITCON新鮮人。國中自學Python，高中在資訊社學C++，參加過一些程式競賽被隊友carry。喜歡學新東西，最近在學組合語言還有火舞，還有在一個小社團裡寫網站後端。偶爾打打CTF，對系統底層比較有興趣。常吃開源社雞排，夢想是找到新竹美食。</p>
      </template>
      <template v-slot:content>
        <p>
          投影片連結
          <a href="https://slides.com/soyccan/pip/">https://slides.com/soyccan/pip/</a><br>
          共筆連結
          <a href="https://hackmd.io/f_a6m_W0RGGgTk4Ez_Xv9w">https://hackmd.io/f_a6m_W0RGGgTk4Ez_Xv9w</a>
        </p>
        <p>可能有人會聽過網路爬蟲這個詞，卻對牠沒有概念。牠是一類程式腳本的統稱，目的是自動從網路抓東西下來，為了取得需要的資料，比如文字，圖片，影音等。Python的原意是蠎蛇，蛇從虫部，在古代被視為廣義的蟲類，在現代則歸為爬蟲類，所以拿牠來寫強大的爬蟲也是很合理的。這堂課會教各位向一個網站請求資料，而要拿取回的資料做什麼應用，就由各位的創意和雙手完成，會很有成就感的。</p>
        <ul>
          <li>The Python Package Installer</li>
          <ul>
            <li>我都念pip</li>
            <li>認識Python超強大的套件庫</li>
            <li>有現成工具用，少奮鬥數個夜晚</li>
          </ul>
          <li>requests – 抓資料起手式</li>
          <ul>
            <li>活用HTTP Requests</li>
          </ul>
          <li>JSON – 萃取需要的資料</li>
        </ul>
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
