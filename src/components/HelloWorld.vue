<template>
  <div class="hello">
    <DetailView ref="detail">
      <day1t12 :hidden="selected!='day1t12'" />
      <day1t22 :hidden="selected!='day1t22'" />
      <day2t3 :hidden="selected!='day2t3'" />
      <day2t14 :hidden="selected!='day2t14'" />
      <day3t3 :hidden="selected!='day3t3'" />
      <day3t14 :hidden="selected!='day3t14'" />
      <day1telegram :hidden="selected!='day1telegram'" />
      <day2security :hidden="selected!='day2security'" />
      <day3infoview :hidden="selected!='day3infoview'" />
      <day4coffee :hidden="selected!='day4coffee'" />
      <day4community :hidden="selected!='day4community'" />
      <day4opensource :hidden="selected!='day4opensource'" />
    </DetailView>

    <div class="container">
      <p>|</p>
      <div
        id="about"
        class="anchor"
      />
      <h2 v-scroll-reveal>
        關於夏令營
      </h2>
      <div
        v-scroll-reveal
        class="page"
      >
        <p>有鑑於資訊領域逐漸成為科技時代的重要學門，社群與開源精神亦持續抬頭，SITCON 團隊認為將資訊教育向下扎根，為在資訊科學領域有興趣的學生提供一個親切而良好的機會入門，並播灑開源種子，是一件相當重要且值得去做的事情。</p>

        <p>
          2014 年至今，SITCON 夏令營已將邁入第五屆，在此之前課程內容涵蓋開源碼、資訊安全、Maker、Python、後端的
          Node.js、前端的資料爬蟲、視覺化等，更有社群闖關、視界咖啡館、黑客松等活動，讓學員充分吸收新知、動手實作、尋找自己的愛好及興趣，進而加入我們一起推動 Open Source。
        </p>

        <p>
          2019 年度，SITCON
          夏令營將於海洋大學舉辦，以「浸身資訊流，征服開源星」為主軸，帶領各位一同進入開源宇宙。承接開源城的概念，今年的開源宇宙將會有介紹社群精神、開源文化、資訊安全等議題的廣度課程，並透過社群闖關讓學員更加了解各個社群的理念、運作，也會有從基礎
          Python 程式語言到做出自己的聊天機器人的實作課程。開源宇宙也將更進一步把故事和營隊整合，配合豐富的課程、座談會及社群闖關，營造完整的體驗，絕對能讓學員擁有截然不同的營隊體驗。
        </p>
      </div>

      <h2 v-scroll-reveal>
        關於 SITCON
      </h2>
      <div
        v-scroll-reveal
        class="page"
      >
        <p>
          學生計算機年會（SITCON）以學生為本、由學生自發舉辦，長期投身學生資訊教育與推廣開源精神，希望引領更多學子踏入資訊的殿堂，更冀望所有對資訊有興趣的學生，能夠在年會裏齊聚一堂，彼此激盪、傳承、啟發，達到「學以致用、教學相長」的實際展現。SITCON
          也是一個屬於學生的舞台，讓學子們實踐、體驗開源社群精神：開放、分享、協作，貢獻一己之長一同讓 SITCON 更好。SITCON 也提供發表自身所學所長的舞台，讓更多人看見你的努力、你的改變！
        </p>
        <p>即使你不會寫程式，但總有你可以做的事！不要害羞，現在就加入我們吧！</p>
      </div>
      <div
        id="course"
        class="anchor"
      />
      <h2 v-scroll-reveal>
        課程
      </h2>
      <div v-scroll-reveal>
        <time-table @selected="classSelect" />
      </div>

      <div class="row">
        <div class="col-6-md">
          <div
            v-scroll-reveal
            class="page course"
          >
            <h3>廣度課程與短講</h3>
            <p>
              今年夏令營有別於往年的單一教學方式，而是在不影響一般課程的情況，安排一些廣度課程，讓學員在學習基礎課程之餘，也能學到資訊領域的其他層面，增加自身資訊技能的廣度。
              除基礎課程與廣度課程外，我們也邀請到許多在資訊領域打滾多年的人士分享自身經驗，期許迷茫中的學員，可以點燃未來的一盞明燈，在資訊道路上有前進的動力及方向。
            </p>
          </div>

          <div
            v-scroll-reveal
            class="page course"
          >
            <h3>社群闖關</h3>
            <p>社群闖關邀請到許多資訊相關社群前來擺攤，藉由互動遊戲、影片欣賞、專人介紹…等方式，讓學員認識所謂「社群」，並對開源活動有初步了解。點選課表可檢視詳細的社群資訊。</p>
          </div>
        </div>
        <div class="col-6-md">
          <div
            v-scroll-reveal
            class="page course"
          >
            <h3>視界咖啡館</h3>
            <p>
              視界咖啡館參考自世界咖啡館（The World Café），在本次夏令營中，我們邀請到各領域及社群前輩，將傳統座談會形式改以小組討論的樣貌呈現，並與學員分享工作經驗、學習過程、面對困難的解決方式或希望給予
              SITCON
              夏令營學員的建議，提出值得學員思考、了解的觀點。期望透過縮短講師及學員間的距離，鼓勵學員踴躍提問、參與，進而產生良好的雙向交流。
            </p>
          </div>

          <div
            v-scroll-reveal
            class="page course"
          >
            <h3>Hackathon</h3>
            <p>黑客松（Hackathon）是「黑客」（Hack；原指早期為電腦系統找尋不完美的地方，或是探索不同的解法，來改善電腦系統）跟「馬拉松」（Marathon）的組合字，顧名思義，也就像是程式設計、工程界的馬拉松。由有興趣的一群人在有限的時間內，發揮自己的專長做出一個有特色的專案。</p>
          </div>
        </div>
      </div>

      <div class="container">
        <h4>
          今年，SITCON 夏令營將為學員
          <br class="if-mobile">打造一場專屬的小型黑客松，
          <br>取代傳統的晚會、唱歌跳舞等活動，
          <br class="if-mobile">以小隊為單位，
          <br>在吃吃喝喝的同時，
          <br class="if-mobile">一起發揮創意、運用課程中所學，
          <br>做出與眾不同的作品呈現！
        </h4>
      </div>
      <div
        id="exp"
        class="anchor"
      />
      <studentexp />
      <div
        id="signup"
        class="anchor"
      />
      <h2 v-scroll-reveal>
        報名
      </h2>
      <div
        v-scroll-reveal
        class="page"
      >
        <h4>活動費用</h4>
        <div class="row">
          <div class="col-6">
            <h5>個人報名</h5>6500 元 /人
          </div>
          <div class="col-6">
            <h5>團隊報名</h5>5900 元 /人
          </div>
        </div>
        <hr>
        <p>
          三人同時報名，視為團體報名，每團以三人為限，請詳閱
          <a
            href="https://drive.google.com/file/d/1YfxLL2Kg6AG1Ol3i_ecgu_4SweCiBI0H/view"
          >活動報名簡章。</a>
        </p>
        <p>本次夏令營預計招收學員 60 名，我們會針對報名資料做簡易審查，非先報先贏。</p>
        <p>正取學員名單將於 2019 / 06 / 18 公佈，正取學員需完成報名費繳交，始完成報名程序。</p>
        <p>
          另設有補助名額，請詳閱
          <a
            href="https://drive.google.com/file/d/1nHNMDzgDH8s7isxoH0_8mF8gIVP2lo5p/view"
          >補助辦法</a>。
        </p>
        <p>
          關於退費事宜，請見
          <a
            href="https://docs.google.com/document/d/1-2yYZS-Hv0ntQ1zA5MCu8bIzXgXWOGVzTvCCXystmVA"
          >退費說明文件</a>。
        </p>
        <hr>
        <h4>報名時間</h4>
        <h5>2019 / 06 / 07 止</h5>
        <a
          href="https://sitcon.kktix.cc/events/sitcon-camp2019"
          target="blank"
        >
          <button disabled>立即報名（已截止）</button>
        </a>
        <h4>報名資格</h4>
        <h5>
          具有學生身分
          <br>（持有任一學生證蓋有 107 學年度上學期註冊章）
          <br>或出生日期為 2000 年 9 月 1 日（含）以後。
        </h5>

        <div class="row">
          <div class="col-6-md">
            <h4>活動時間</h4>
            <h5>
              8/7（三） ~ 8/11（日）
              <br>（五天四夜，含住宿）
            </h5>
          </div>
          <div class="col-6-md">
            <h4>活動地點</h4>
            <h5>
              國立臺灣海洋大學
              <br>
              <a href="https://goo.gl/maps/UZ9cUuJiVxAtDiAk6">（202基隆市中正區北寧路2號）</a>
            </h5>
          </div>
        </div>

        <h4>注意事項</h4>
        <ul>
          <li>
            本次活動採用 KKTIX 售票進行報名，請詳細閱讀
            <a
              href="https://drive.google.com/file/d/1YfxLL2Kg6AG1Ol3i_ecgu_4SweCiBI0H/view"
            >活動報名簡章</a>。
          </li>
          <li>正式取得學員資格後不得轉讓予他人使用，轉讓者將取消資格。</li>
          <li>繳費完成始完成報名程序，正取學員若未於期限內繳交報名費用，將取消資格，由備取者遞補。</li>
          <li>錄取通知以及行前注意等資訊，均將透過報名時所留下之電子郵件通知學員，請務必定期檢查信箱，以確保個人權益。</li>
          <li>團體報名不保證所有團員皆錄取，唯團報經錄取者，皆可享有團體報名優惠。</li>
          <li>
            有任何問題歡迎來信至
            <a href="mailto:ask@sitcon.camp">ask@sitcon.camp</a>
            ， 我們將儘速回覆您。
          </li>
        </ul>
      </div>

      <div
        id="code-of-conduct"
        class="anchor"
      />

      <h2 v-scroll-reveal>
        行為準則
        <br>Code of Conduct
      </h2>
      <div
        v-scroll-reveal
        class="page"
      >
        <p>
          SITCON 夏令營期許成為年輕學子踏入資訊世界的引路人，同時我們也致力於為每位成員提供更友善、開放的環境。相信每位進入 SITCON 夏令營的學員及夥伴都值得被尊重，而我們亦將盡力提供最安全的環境，讓參與
          SITCON 夏令營的每個人能夠尊重個體間的差異、在社群中相互扶助、並鼓勵所有人揮灑屬於自己的生命色彩。 因此，若有幸能在 SITCON
          夏令營與您見面，無論您是以學員、贊助商、工作人員、或是講者的身份參加，我們都希望您配合遵守以下的行為準則：
        </p>
        <ul>
          <li>尊重每一位參與者，將對方的感受放在心上。</li>
          <li>避免使用帶有侮辱、歧視、或具有潛在騷擾意涵的言語及手勢。</li>
          <li>多關心周遭的所有同伴，適度詢問對方是否需要協助。</li>
          <li>當遭遇危險、或發現事情不對勁時，適時尋求工作人員的支援與協助。</li>
          <li>在夏令營裡多交朋友，珍惜彼此相聚的時光！</li>
        </ul>
      </div>
      <div
        v-scroll-reveal
        class="page"
      >
        <h4>以下的行為是不被容忍的：</h4>
        <ul>
          <li>針對性別、性向、種族、外貌、宗教、年齡、身體狀況或個人身份的挑釁或冒犯。</li>
          <li>任何形式的性騷擾、言語及肢體霸凌。</li>
          <li>公開發表、展示或放映含有侮辱、歧視、仇恨、暴力、或是性暗示的言論、影像、或錄影。</li>
          <li>無故干擾課程、議程或活動的正常進行，無視工作人員或他人的制止。</li>
          <li>干擾、攻擊現場提供之網路，未經同意側錄封包或散佈隱私資訊。</li>
          <li>任何違反法律的行為。</li>
        </ul>
      </div>
      <div
        v-scroll-reveal
        class="page"
      >
        <p>為了確保每位參與者的安全，我們將恪守以上規則。</p>
        <p>
          對於違反行為準則者，我們將採取必要且合理的手段予以介入，包含但不限於將參與者請離現場、自相關名冊除名或列為不受歡迎對象，或在必要時移送警察機關法辦。
          若您或他人遇到了以上情況、或是有任何其他顧慮，都請立即尋求 SITCON 夏令營工作人員的協助。
        </p>
        <p>
          我們誠摯的邀請來到 SITCON 夏令營的朋友一同履行以上承諾，將 SITCON 夏令營打造為更友善、溫暖的所在；
          讓每一位參與者，都能在夏令營的活動和相處中共同成長、在人與人的互動中找到自信——而這正是我們所珍惜、試圖給予所有學員的，屬於學生社群的真正精神。
        </p>
      </div>
      <div
        id="staff"
        class="anchor"
      />
      <h2 v-scroll-reveal>
        工作人員
      </h2>
      <div
        v-scroll-reveal
        class="page"
      >
        <p class="staff">
          總召組：魯蛋、黑楓、家維
          行政組：葉子、球魚、揪凱
          課活組：鯉魚、IU、野足、OuO、阿軒、秉虎、君翰、柏凱、雷電芽衣、球魚、William Mou、小t、樹懶、YAYA
          編輯組：Paul、樹懶
          文創組：火柴、Yue、一一、William Mou、小t、阿江
          庶務組：練練、功逸、可晴、阿江、小雲豹
          攝影組：小草、月太、小涼、Jeffrey Lin家康
          財務組：小學生、Han
          行銷組：Denny
          隊輔組：拉布、寶寶、YC、Sean、腋毛、Vense、凱凱、去冰、肥貓、Allen Chou、小知、任禎、欣岑、宙斯、雷孟、vana、Trista、彥伊、鈺婷、Rong、古哥、攤攤
        </p>
      </div>
      <!-- footer -->
    </div>

    <footer>
      <div class="container">
        <div class="logo-list">
          <div class="item">
            <img
              src="../assets/itsa.png"
              alt
            >
          </div>
          <div class="item small">
            <img
              src="../assets/海洋大學.png"
              alt
            >
          </div>
          <div class="item">
            <img
              src="../assets/海大資工.png"
              alt
            >
          </div>
          <div class="item">
            <img
              src="../assets/ocf.png"
              alt
            >
          </div>
          <div class="item">
            <img
              src="../assets/logo.png"
              alt
            >
          </div>
        </div>
        <p>SITCON 學生計算機年會 / SITCON 夏令營</p>
      </div>
    </footer>
  </div>
</template>

<script>
import TimeTable from './TimeTable.vue'
import studentexp from './studentexp.vue'
import DetailView from './DetailView'

import day1t12 from './contents/day1t12.vue'
import day1t22 from './contents/day1t22.vue'
import day1telegram from './contents/day1telegram'
import day2security from './contents/day2security.vue'
import day3infoview from './contents/day3infoview.vue'
import day4coffee from './contents/day4coffee.vue'
import day4community from './contents/day4community.vue'
import day4opensource from './contents/day4opensource.vue'
import day2t3 from './contents/day2t3.vue'
import day2t14 from './contents/day2t14.vue'
import day3t3 from './contents/day3t3.vue'
import day3t14 from './contents/day3t14.vue'

// import { truncate } from 'fs'
var classDetails = {
  day1t12,
  day1t22,
  day2t3,
  day2t14,
  day3t3,
  day3t14,
  day1telegram,
  day2security,
  day3infoview,
  day4coffee,
  day4community,
  day4opensource
}

export default {
  name: 'HelloWorld',
  components: {
    TimeTable,
    studentexp,
    DetailView,
    // contents
    day1t12,
    day1t22,
    day2t3,
    day2t14,
    day3t3,
    day3t14,
    day1telegram,
    day2security,
    day3infoview,
    day4coffee,
    day4community,
    day4opensource
  },
  data () {
    return {
      selected: null
    }
  },
  mounted () {},
  methods: {
    classSelect (c) {
      this.selected = c
      if (classDetails[this.selected]) this.$refs['detail'].display = true
      console.log(this.selected)
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../style/main.scss";

.page {
  border: solid 1px white;
  border-radius: 32px;
  padding: 20px 16px;
  margin: 16px 0px 0px;
  background: rgba(255, 255, 255, 0.9);
  color: black;

  box-sizing: border-box;

  p {
    text-align: left;
  }

  h3 {
    margin-top: 20px;
  }

  @include rwd-below(768px) {
    padding: 8px 4px;
  }

  @include rwd-above(768px) {
    &.course {
      min-height: 320px;
    }
  }
}

.logo-list {
  display: flex;
  align-items: center;
  .item {
    width: 20%;
    margin: 8px;
    box-sizing: border-box;
    img {
      top: 50%;
      width: 100%;
    }
    &.small {
      padding: 2%;
    }
  }
}

.staff {
  white-space: pre-line;
  text-align: left;
}

footer {
  margin-top: 64px;
  background: rgba(255, 255, 255, 0.9);
  padding-top: 16px;
  padding-bottom: 32px;
  color: black;
}
</style>
