<template>
  <div>
    <DetailFormat>
      <template v-slot:title>
        Python function 系列、Review
      </template>
      <template v-slot:subtitle>
        Day 2 14:30 - 17:30 (3hr)
      </template>
      <template v-slot:teacher>
        林君翰
      </template>
      <template v-slot:desc>
        <p>
          海大資工大三，曾在ICPC亞洲區花蓮站以及各種大大小小的程式競賽獲得佳作（對沒錯，都是佳作QQ）。
          自學 Python 直到有一天悟道而變成 Python 教徒。
          經歷豐富，曾在 6/4 的前一天被大學選課迫害，同時也是個底線王與編曲菜雞。
          不具有記憶能力、常常需要室友幫忙找東西。
        </p>
      </template>
      <template v-slot:content>
        <p>
          投影片連結
          <a href="https://drive.google.com/open?id=1hiDrAX_Zv_BxB5NiyTZfcbStPtSgYt_T">https://drive.google.com/open?id=1hiDrAX_Zv_BxB5NiyTZfcbStPtSgYt_T</a>
        </p>
        <p>
          常常寫了幾百行 code 卻發現裡面有一半都是重複的嗎？
          昨天寫的 code 今天就忘了他們在幹嘛了嗎？
          想叫同學幫你寫作業卻發現溝通起來有障礙嗎？
          這堂課將會介紹 Python 中的 function，讓你把你寫好的 code 全部打包帶走！
        </p>

        <ul>
          <li>function</li>
          <ul>
            <li>基本 function 語法、觀念</li>
            <li>function 中的區域變數</li>
          </ul>
          <li>與他人共作</li>
          <ul>
            <li>module</li>
            <li>介面溝通</li>
          </ul>
          <li>「等等...昨天講了什麼我有點忘了QQ」沒關係！皮諾可，這個直接電死。</li>
          <ul>
            <li>皮諾可幫你複習</li>
          </ul>
        </ul>
      </template>
      <template v-slot:image>
        <img
          src="../../assets/teachers/君翰.jpg"
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
