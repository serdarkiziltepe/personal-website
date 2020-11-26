<template>
  <div id="page">
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
            "https://cdnjs.cloudflare.com/ajax/libs/jquery/3.1.1/jquery.min.js",
        },
      ],
      link: [
        {
          rel: "stylesheet",
          href:
            "https://fonts.googleapis.com/css2?family=Varela+Round&display=swap",
        },
        {
          rel: "stylesheet",
          href: "https://use.fontawesome.com/releases/v5.13.0/css/all.css",
        },
      ],
    };
  },
};
</script>



<style lang="scss">
html {
  // font-family: "Rasa", serif;
  font-family: "Varela Round", sans-serif;
  font-size: 16px;
  overflow: hidden;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

#page {
  height: 100vh;
  overflow: hidden;
}

$color-bg: #ebecf0;
$white: #ffffff;
$black: #000;
$soft-gray: #61677c;
$red: #ae1100;
$blue-soft: #253441;

$primary-text-color: #a3b1c6;

a {
  text-decoration: none;
}

.links {
  display: inline-flex;
  margin: 0 10px;
}

body {
  width: 100%;
  height: 100%;
  background-color: $color-bg;
  line-height: 1.6;
  position: relative;

  cursor: red;
}

.button-green {
  display: inline-block;
  border-radius: 4px;
  color: $soft-gray;
  text-decoration: none;
  font-weight: bold;
  padding: 15px 50px;

  box-shadow: -2px -2px 5px white, 2px 2px 5px #babecc;
  transition: all 0.2s ease-in-out;
  &:hover {
    background: #ebecf0;
    box-shadow: -5px -5px 20px white, 5px 5px 20px #babecc;
  }

  &:active {
    box-shadow: inset 5px 5px 10px #d6d7da, inset -5px -5px 10px #ffffff;
  }
}

.container {
  max-width: 1234px;
  margin-left: auto;
  margin-right: auto;
  width: 95%;
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
    width: 1.3px;
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
        $red 75%,
        $red 100%
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

.social-media {
  position: absolute;
  bottom: 50px;
  right: 50px;
  animation: 4s appear;

  ul {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr 1fr 1fr 1fr;
    gap: 15px;

    li {
      background-color: #ebecf0;
      text-shadow: 1px 1px 0 white;

      box-shadow: -2px -2px 5px white, 2px 2px 5px #babecc;
      transition: all 0.2s ease-in-out;
      cursor: pointer;
      font-weight: 600;

      height: 50px;
      width: 50px;

      display: flex;
      align-items: center;
      justify-content: center;

      border-radius: 8px;

      &:hover {
        box-shadow: -5px -5px 20px white, 5px 5px 20px #babecc;
      }

      a {
        i {
          color: #61677c;
          font-size: 25px;
        }
      }
    }
  }
}
</style>
