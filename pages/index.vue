<template>
  <div class="container">
    <div class="lines">
      <div class="line"></div>
      <div class="line"></div>
      <div class="line"></div>
    </div>

    <div class="background-svg">
      <div class="oval"></div>
      <div class="oval-2"></div>
      <div class="oval-3"></div>
      <!-- <div class="oval-4"></div>
      <div class="oval-5"></div>-->
    </div>

    <div class="content">
      <!-- <h1 class="title">
        Serdar Landing
      </h1>-->
      <h2 class="subtitle">Hi, I'm Serdar KIZILTEPE,</h2>
      <p>I'm a Web Developer.</p>
      <div class="links">
        <a
          href="mailto:serdar.kiziltepe@gmail.com"
          target="_blank"
          class="button-green"
          >CONTACT</a
        >
      </div>
      <!-- <div class="links">
        <nuxt-link to="/periodic-table" class="button-green">PERIODIC TABLE</nuxt-link>
      </div>-->
    </div>
    <div class="social-media">
      <ul>
        <li>
          <a href="https://www.instagram.com/serdar.kiziltepe/" target="_blank">
            <i class="fab fa-instagram"></i>
          </a>
        </li>
        <li>
          <a href="https://github.com/serdarkiziltepe" target="_blank">
            <i class="fab fa-github"></i>
          </a>
        </li>
        <li>
          <a
            href="https://www.linkedin.com/in/serdarkiziltepe/"
            target="_blank"
          >
            <i class="fab fa-linkedin-in"></i>
          </a>
        </li>
        <li>
          <a
            href="https://www.youtube.com/channel/UCOdkumUmsmGM8-0JMlTYt_Q?view_as=subscriber"
            target="_blank"
          >
            <i class="fab fa-youtube"></i>
          </a>
        </li>
        <li>
          <a
            href="https://www.youtube.com/channel/UCOdkumUmsmGM8-0JMlTYt_Q?view_as=subscriber"
            target="_blank"
          >
            <i class="fab fa-500px"></i>
          </a>
        </li>
        <li>
          <a
            href="https://www.youtube.com/channel/UCOdkumUmsmGM8-0JMlTYt_Q?view_as=subscriber"
            target="_blank"
          >
            <i class="fab fa-twitter"></i>
          </a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
import Logo from "~/components/Logo.vue";
import Header from "~/components/Header.vue";

export default {
  components: {
    Logo,
    Header,
  },
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
  font-size: 60px;
  color: #61677c;
  word-spacing: 5px;
  opacity: 0.9;
  text-shadow: 5px 5px 20px white, -5px -5px 20px #babecc;
}

p {
  color: #61677c;
  font-size: 40px;
  margin-top: 0;
  opacity: 0.9;
}

.links {
  padding-top: 15px;
}

// BG ANIMATON
.background-svg {
  position: absolute;
  left: -300px;
  z-index: -2;
}

.oval {
  border-radius: 100%;
  position: absolute;

  background: #ebecf0;
  box-shadow: inset 5px 5px 10px #d6d7da, inset -5px -5px 10px #ffffff;

  width: 40em;
  height: 40em;
  position: absolute;
  top: -8.5em;
  left: -1em;
  animation: 3s appear;
}

.oval-2 {
  position: absolute;
  border-radius: 100%;
  background: #ebecf0;
  box-shadow: inset 5px 5px 10px #d6d7da, inset -5px -5px 10px #ffffff;
  animation: 8s appear;

  width: 40em;
  height: 40em;
  position: absolute;
  bottom: -5em;
  left: 4em;
}

.oval-3 {
  position: absolute;
  border-radius: 100%;
  background: #ebecf0;
  box-shadow: inset 5px 5px 10px #d6d7da, inset -5px -5px 10px #ffffff;

  width: 40em;
  height: 40em;
  position: absolute;
  bottom: -22em;
  left: -12em;
}

.oval-4 {
  position: absolute;
  border-radius: 100%;
  background: #ebecf0;
  box-shadow: inset 5px 5px 10px #d6d7da, inset -5px -5px 10px #ffffff;

  width: 40em;
  height: 40em;
  position: absolute;
  bottom: -20em;
  left: 5em;
  z-index: -1;
}

.oval-5 {
  position: absolute;
  border-radius: 100%;
  background: #ebecf0;
  box-shadow: inset 5px 5px 10px #d6d7da, inset -5px -5px 10px #ffffff;
  width: 40em;
  height: 40em;
  position: absolute;
  top: -45em;
  left: 0em;
  z-index: 1;
}
</style>
