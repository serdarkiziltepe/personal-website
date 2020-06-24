<template>
  <div class="container">
    <!-- Thanks OSORINA IRINA for Animation Codes // Codepen @333397406 -->

    <Header />

    <div class="lines">
      <div class="line"></div>
      <div class="line"></div>
      <div class="line"></div>
    </div>

    <div class="content">
      <!-- <h1 class="title">
        Serdar Landing
      </h1>-->
      <h2 class="subtitle">Hi, I'm Serdar KIZILTEPE,</h2>
      <p>I'm a Web Developer.</p>
      <div class="links">
        <a href="mailto:serdar.kiziltepe@gmail.com" target="_blank" class="button--white">CONTACT</a>
      </div>
    </div>
    <div class="social-media">
      <a href="https://www.instagram.com/serdar.kiziltepe/" target="_blank">
        <i class="fab fa-instagram"></i>
      </a>
      <a href="https://github.com/serdarkiziltepe" target="_blank">
        <i class="fab fa-github"></i>
      </a>
      <a href="https://www.linkedin.com/in/serdarkiziltepe/" target="_blank">
        <i class="fab fa-linkedin-in"></i>
      </a>
      <a
        href="https://www.youtube.com/channel/UCOdkumUmsmGM8-0JMlTYt_Q?view_as=subscriber"
        target="_blank"
      >
        <i class="fab fa-youtube"></i>
      </a>
    </div>
  </div>
</template>

<script>
import Logo from "~/components/Logo.vue";
import Header from "~/components/Header.vue";

export default {
  components: {
    Logo,
    Header
  }
};
</script>

<style  lang="scss">
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.content {
  text-align: left;
  animation: 2s appear;
}

.title {
  display: block;
  font-weight: 300;
  font-size: 80px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  text-align: left;
  font-weight: 300;
  font-size: 50px;
  color: #f5f5f5;
  word-spacing: 5px;
  opacity: 0.9;
}

p {
  color: #f5f5f5;
  font-size: 40px;
  margin-top: 0;
  opacity: 0.9;
}

.links {
  padding-top: 15px;
}
</style>
