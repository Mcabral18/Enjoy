<template>
  <div id="app">
    <section class="home_page" :class="{ active: toggleMenu == true }">
      <header>
        <h2 class="logo">Enjoy</h2>
        <div
          class="toggle"
          @click="toggleMenu = !toggleMenu"
          :class="{ active: toggleMenu == true }"
        ></div>
      </header>
      <video
        src="./assets/Pexels Videos 1739010.mp4"
        muted
        loop
        autoplay
      ></video>
      <div class="overlay"></div>
      <div class="slogan">
        <h2>wonderful experiences</h2>
        <h3>Explore the world</h3>
        <p>"Live life to the fullest, and focus on the positive"</p>
        <a href="#">Explore</a>
      </div>
      <ul class="social">
        <li>
          <a href="#"><img src="https://i.ibb.co/x7P24fL/facebook.png" /></a>
        </li>
        <li>
          <a href="#"><img src="https://i.ibb.co/Wnxq2Nq/twitter.png" /></a>
        </li>
        <li>
          <a href="#"><img src="https://i.ibb.co/ySwtH4B/instagram.png" /></a>
        </li>
      </ul>
    </section>
    <div class="menu">
      <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">News</a></li>
        <li><a href="#">Blog</a></li>
        <li><a href="#">Contact</a></li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      toggleMenu: false,
    };
  },
};
</script>

<style src="./assets/style.css">
</style>
