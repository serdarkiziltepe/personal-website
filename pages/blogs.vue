<template>
  <div class="container">
    <div class="blog">
      <h1 class="title">Blogs</h1>
      <ul>
        <li onclick="myFunction()" v-for="post in posts" :key="post.id">
          <h1>{{ post.title }}</h1>
          <p>{{ post.content }}</p>
        </li>
      </ul>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      posts: [
        {
          id: "fizik",
          title: "Neomorphic Design",
          content:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Quibusdam, facere. Harum cupiditate accusantium omnis consequatur. Facilis expedita illum quibusdam repellat debitis a suscipit aliquid nesciunt harum. Eos delectus at quae?"
        },

        {
          id: "kimya",
          title: "Kimya nedir?",
          content:
            "Kimya Görünenin içini araştır Lorem ipsum dolor sit amet consectetur adipisicing elit. Quibusdam, facere. Harum cupiditate accusantium omnis consequatur. Facilis expedita illum quibusdam repellat debitis a suscipit aliquid nesciunt harum. Eos delectus at quae?"
        },

        {
          id: "kimya",
          title: "Kimya nedir?",
          content:
            "Kimya Görünenin içini araştır Lorem ipsum dolor sit amet consectetur adipisicing elit. Quibusdam, facere. Harum cupiditate accusantium omnis consequatur. Facilis expedita illum quibusdam repellat debitis a suscipit aliquid nesciunt harum. Eos delectus at quae?"
        },

        {
          id: "biyoloji",
          title: "Biyoloji nedir?",
          content:
            "Canlı bilimidir Lorem ipsum dolor sit amet consectetur adipisicing elit. Quibusdam, facere. Harum cupiditate accusantium omnis consequatur. Facilis expedita illum quibusdam repellat debitis a suscipit aliquid nesciunt harum. Eos delectus at quae?"
        }
      ]
    };
  }
};
</script>

<style lang="scss">
.blog {
  .title {
    margin: 20px;
    text-align: center;
  }

  ul {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    gap: 30px;

    li {
      background-color: #ebecf0;
      padding: 30px 60px;

      list-style: none;

      box-shadow: 9px 9px 16px rgba(163, 177, 198, 0.6),
        -9px -9px 16px rgba(255, 255, 255, 0.5),
        inset 3px 3px 7px rgba(136, 165, 191, 0.48), inset -3px -3px 7px #ffffff;
      background: linear-gradient(
        318.32deg,
        rgba(163, 177, 198, 0.1) 0%,
        rgba(163, 177, 198, 0.1) 55%,
        rgba(163, 177, 198, 0.25) 100%
      );
    }

    h1 {
      color: #ae1100;
    }
  }
}
</style>
