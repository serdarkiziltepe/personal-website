<template>
  <div>
    <nuxt />
  </div>
</template>


<script>
export default {
  head() {
    return {
      script: [
        {
          src:
            "https://cdnjs.cloudflare.com/ajax/libs/jquery/3.1.1/jquery.min.js"
        }
      ],
      link: [
        {
          rel: "stylesheet",
          href:
            // "https://fonts.googleapis.com/css2?family=Rasa:wght@500&display=swap"
            "https://fonts.googleapis.com/css2?family=Varela+Round&display=swap"
        }
      ]
    };
  }
};
</script>



<style lang="scss">
@import url("https://use.fontawesome.com/releases/v5.13.0/css/all.css");

html {
  // font-family: "Rasa", serif;
  font-family: "Varela Round", sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

.button--green {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #3b8070;
  color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
}

.button--white {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #f5f5f5;
  color: #f5f5f5;
  text-decoration: none;
  padding: 10px 30px;
}

.button--green:hover {
  color: #fff;
  background-color: #3b8070;
}

.button--grey {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #35495e;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}

.button--grey:hover {
  color: #fff;
  background-color: #35495e;
}

.container {
  height: 100vh;
  max-width: 1234px;
  margin-left: auto;
  margin-right: auto;
  width: 95%;
}

body {
  display: table;
  width: 100%;
  height: 100%;
  background-color: black;
  color: #000;
  line-height: 1.6;
  position: relative;
  overflow: hidden;
}

.lines {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 100%;
  margin: auto;
  width: 100vw;
  z-index: -1;
  .line {
    position: absolute;
    width: 1px;
    height: 100%;
    top: 0;
    left: 50%;
    background: rgba(255, 255, 255, 0.1);
    overflow: hidden;
    &::after {
      content: "";
      display: block;
      position: absolute;
      height: 15vh;
      width: 100%;
      top: -50%;
      left: 0;
      background: linear-gradient(
        to bottom,
        rgba(255, 255, 255, 0) 0%,
        #ffffff 75%,
        #ffffff 100%
      );
      animation: run 7s 0s infinite;
      animation-fill-mode: forwards;
      animation-timing-function: cubic-bezier(0.4, 0.26, 0, 0.97);
    }
    &:nth-child(1) {
      margin-left: -25%;
      &::after {
        animation-delay: 2s;
      }
    }
    &:nth-child(3) {
      margin-left: 25%;
      &::after {
        animation-delay: 2.5s;
      }
    }
  }
}

@keyframes run {
  0% {
    top: -50%;
  }
  100% {
    top: 110%;
  }
}

$white: #ffffff;

.social-media {
  position: absolute;
  bottom: 50px;
  right: 50px;
  animation: 4s appear;
  a {
    margin-right: 15px;

    &:last-child {
      margin-right: 0;
    }
    i {
      color: $white;
      font-size: 25px;
    }
  }
}
</style>
