<template>
  <div id="app" class=".slide-in-bottom">
    <div id="container">
      <img id="avatar" alt="avatar" src="./assets/logo1.jpg" />
      <h1>Michael Chu</h1>
      <br>
      <span>开发 / 数字极简 / 手机摄影 / 终生学习</span>
      <br>
      <br>
      <span>
        * I enjoy codes, podcasts, F1 and Tech.
      </span>

      <hr id="top-hr" />
      <h3>Featured Projects</h3>
      <div id="card-container">
        <Card
          msg="GitHub"
          backgroundColor="#24292E"
          textColor="#FFFFFF"
          icon="github.png"
          link="https://github.com/yiukuenchu"
        />
        <Card
          msg="少数派 sspai"
          backgroundColor="#BC1820"
          textColor="#FFFFFF"
          icon="sspai.png"
          link="https://beta.sspai.com/u/uncle/posts"
        />
        <!-- <Card
          msg="Blogs on Medium"
          backgroundColor="#1AA77D"
          textColor="#FFFFFF"
          icon="medium.png"
          link="https://medium.com/coffee-minutes"
        /> -->
      </div>

      <div id="others">
        <hr />
        <h3>You can also find me on:</h3>
        <div class="social-media">
          <div class="social-media-card">
            <img class="media-icon" src="@/assets/500px.png" alt />
            <span>
              500px:
              <a
                href="https://500px.com/yiukuenchu"
              >@yiukuenchu</a>
            </span>
          </div>
          <!-- <div class="social-media-card">
            <img class="media-icon" src="@/assets/weibo.png" alt />
            <span>
              Weibo:
              <a href="https://weibo.com/u/2981748155">@热带阿叔</a>
            </span>
          </div> -->
          <div class="social-media-card">
            <img class="media-icon" src="@/assets/instagram.png" alt />
            <span>
              Instagram:
              <a href="https://www.instagram.com/yiukuenchu/">@yiukuenchu</a>
            </span>
          </div>
          <div class="social-media-card">
            <img class="media-icon" src="@/assets/telegram.png" alt />
            <span>
              Telegram:
              <a href="https://t.me/universe_daily">Universe Daily | 太空日报</a>
            </span>
          </div>
        </div>

        <hr />
        <p>
          Previous blog posts have been archived at:
          <a
            href="https://archive.yiukuenchu.codes"
          >https://archive.yiukuenchu.codes</a>. Thank you for following me.
        </p>
      </div>
    </div>

    <div id="footer">
      <div id="footer-text">©{{ getYear() }} yiukuenchu</div>
    </div>
  </div>
</template>

<script>
import Card from './components/Card.vue'

export default {
  name: 'app',
  components: {
    Card
  },
  methods: {
    getYear() {
      return new Date().getFullYear()
    }
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Miriam+Libre|Rubik&display=swap');

body {
  background-color: #f5f4f1;
  margin: 0;
}

#app {
  font-family: 'Rubik', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #141313;
  -webkit-animation: slide-in-bottom 0.5s cubic-bezier(0.25, 0.46, 0.45, 0.94)
    both;
  animation: slide-in-bottom 0.5s cubic-bezier(0.25, 0.46, 0.45, 0.94) both;
}

#container {
  text-align: center;
  margin: 40px auto 0 auto;
  max-width: 600px;
  padding: 60px 20px;
}

#avatar {
  width: 120px;
  height: 120px;
  border-radius: 60px;
}

h1 {
  font-family: 'Miriam Libre', sans-serif;
  font-weight: 700;
  font-size: 28px;
}

h2 {
  font-weight: 400;
  font-size: 20px;
  padding: 20px 0;
}

h3{
  font-family: 'Miriam Libre', sans-serif;
}

hr {
  width: 100px;
  margin: 60px 0;
  border-top: solid 3px #141313;
}

span {
  color: #666666;
}

#top-hr {
  width: 100px;
  margin: 60px auto;
  border-top: solid 3px #c03237;
}

.social-media-card {
  display: flex;
  align-items: center;
  margin: 20px 0;
}

.social-media-card .media-icon {
  width: 30px;
  height: 30px;
  padding-right: 20px;
}

p{
  font-family: 'Miriam Libre', sans-serif;
}

a {
  text-decoration: none;
  color: #c03237;
}

a:hover {
  border-bottom: #c03237 solid 1px;
}

#others {
  text-align: left;
}

#footer {
  padding: 20px 20px;
  background-color: #141313;
  color: #ffffff;
}

#footer-text {
  margin: 0px auto;
  max-width: 600px;
}

/* ----------------------------------------------
 * Generated by Animista on 2019-7-28 20:57:15
 * w: http://animista.net, t: @cssanimista
 * ---------------------------------------------- */

/**
 * ----------------------------------------
 * animation slide-in-bottom
 * ----------------------------------------
 */
@-webkit-keyframes slide-in-bottom {
  0% {
    -webkit-transform: translateY(1000px);
    transform: translateY(1000px);
    opacity: 0;
  }
  100% {
    -webkit-transform: translateY(0);
    transform: translateY(0);
    opacity: 1;
  }
}
@keyframes slide-in-bottom {
  0% {
    -webkit-transform: translateY(1000px);
    transform: translateY(1000px);
    opacity: 0;
  }
  100% {
    -webkit-transform: translateY(0);
    transform: translateY(0);
    opacity: 1;
  }
}
</style>
