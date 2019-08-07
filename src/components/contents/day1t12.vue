<template>
  <div>
    <DetailFormat>
      <template v-slot:title>
        Python env、VSCode、Python 介紹、基礎語法
      </template>
      <template v-slot:subtitle>
        Day 1 13:30 - 16:30 (3hr)
      </template>
      <template v-slot:teacher>
        柏凱
      </template>
      <template v-slot:desc>
        <p>海洋大學資工系大三，曾參與 ICPC 亞洲區花蓮站並獲得佳作，也曾參與 ITSA 桂冠賽闖關組也獲得佳作 (其他比賽也都是佳作 QQ)。正在往仙人邁進的大學生，因為室友沒有甚麼記憶能力，所以很擅長幫室友找東西。</p>
      </template>
      <template v-slot:content>
        <p>
          投影片連結
          <a href="https://slides.com/adkevin3307/python-3/#/">https://slides.com/adkevin3307/python-3/#/</a>
        </p>
        <p>
          <strike>常言道：珍惜生命，請用 Python。</strike>
        </p>
        <p>相信很多人都聽過 Python 這門程式語言，那 Python 究竟是甚麼，它為甚麼讓很多人愛不釋手，透過這堂課來開始認識 Python 吧~</p>
        <ul>
          <li>Python3 環境介紹</li>
          <li>介紹 VSCode (以下開放大家戰編輯器</li>
          <li>Python3 基礎語法</li>
          <ul>
            <li>基本資料型態</li>
            <li>變數是甚麼，能吃嗎</li>
            <li>if-else</li>
            <li>for-while</li>
          </ul>
        </ul>
      </template>
      <template v-slot:image>
        <img
          src="../../assets/teachers/柏凱.jpg"
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
