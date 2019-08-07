<template>
  <div>
    <DetailFormat>
      <template v-slot:title>
        Python 基礎資料結構(list / dict / tuple)
      </template>
      <template v-slot:subtitle>
        Day 1 18:30 - 21:30 (3hr)
      </template>
      <template v-slot:teacher>
        火箭隊
      </template>
      <template v-slot:desc>
        <p>既然你誠心誠意地請教了，那我就先不要告訴你：）</p>
      </template>
      <template v-slot:content>
        <p>
          投影片連結
          <a href="https://drive.google.com/file/d/1NRpXeZfOZ212vlPyHzxBhJR8BEAXgp6r/view?usp=sharing">https://drive.google.com/file/d/1NRpXeZfOZ212vlPyHzxBhJR8BEAXgp6r/view?usp=sharing</a>
        </p>
        <p>如果只有變數好像成不了大事，要記住很多內容的時候該怎麼辦？這堂課將會教你如何利用 Python 中的 container 讓你把想要的資料都全給存起來！</p>
        <ul>
          <li>Container in Python3</li>
          <ul>
            <li>list</li>
            <li>dict</li>
            <li>tuple</li>
          </ul>
        </ul>
      </template>
      <template v-slot:image>
        <img
          src="../../assets/teachers/火箭隊.jpg"
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
