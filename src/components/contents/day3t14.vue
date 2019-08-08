<template>
  <div>
    <DetailFormat>
      <template v-slot:title>
        telegram bot
      </template>
      <template v-slot:subtitle>
        Day 3 14:30 - 17:30 (3hr)
      </template>
      <template v-slot:teacher>
        黑楓
      </template>
      <template v-slot:desc>
        <p>北科大資工系四年級，曾任北科程式設計研究社 1st 社長。平常喜歡不務正業的寫和學校無關的程式，偶爾寫一些小服務、開發一些 App、打打 CTF 的小廢廢。</p>
      </template>
      <template v-slot:content>
        <p>
          投影片
          <a href="https://drive.google.com/open?id=1Cd12jOW74tjOFYGEhS6cnr5gbGJmiPdl">https://drive.google.com/open?id=1Cd12jOW74tjOFYGEhS6cnr5gbGJmiPdl</a><br>
          共筆
          <a href="https://hackmd.io/amX5HnbdSLC-JOFsOar2hg">https://hackmd.io/amX5HnbdSLC-JOFsOar2hg</a>
        </p>
        <p>可能有人會聽過網路爬蟲這個詞，卻對牠沒有概念。牠是一類程式腳本的統稱，目的是自動從網路抓東西下來，為了取得需要的資料，比如文字，圖片，影音等。Python的原意是蠎蛇，蛇從虫部，在古代被視為廣義的蟲類，在現代則歸為爬蟲類，所以拿牠來寫強大的爬蟲也是很合理的。這堂課會教各位向一個網站請求資料，而要拿取回的資料做什麼應用，就由各位的創意和雙手完成，會很有成就感的。</p>
        <ul>
          <li>Telegram</li>
          <ul>
            <li>介紹</li>
            <li>vs Line</li>
          </ul>
          <li>聊天機器人 Bot</li>
          <li>Telegram API</li>
          <ul>
            <li>Client API</li>
            <li>Bot API</li>
          </ul>
          <li>python-telegram-bot - A Python framework for Telegram Bot API</li>
          <li>簡單實作</li>
        </ul>
      </template>
      <template v-slot:image>
        <img
          src="../../assets/teachers/黑楓.jpg"
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
