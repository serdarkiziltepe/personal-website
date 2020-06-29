<template>
  <div class="container">
    <!-- <Header /> -->
    <div class="sigle-blog">
      <h1>{{ post.title }}</h1>
      <p>{{ post.content }}</p>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      id: this.$route.params.id,

      posts: [
        {
          id: "fizik",
          title: "Fizik nedir?",
          content:
            "Fizik Görüneni araştırır Lorem ipsum dolor sit amet consectetur adipisicing elit. Quibusdam, facere. Harum cupiditate accusantium omnis consequatur. Facilis expedita illum quibusdam repellat debitis a suscipit aliquid nesciunt harum. Eos delectus at quae?"
        },

        {
          id: "kimya",
          title: "Kimya nedir?",
          content:
            "Kimya Görünenin içini araştır Lorem ipsum dolor sit amet consectetur adipisicing elit. Quibusdam, facere. Harum cupiditate accusantium omnis consequatur. Facilis expedita illum quibusdam repellat debitis a suscipit aliquid nesciunt harum. Eos delectus at quae?"
        },

        {
          id: "biyoloji",
          title: "Bİyoloji nedir?",
          content:
            "Canlı bilimidir Lorem ipsum dolor sit amet consectetur adipisicing elit. Quibusdam, facere. Harum cupiditate accusantium omnis consequatur. Facilis expedita illum quibusdam repellat debitis a suscipit aliquid nesciunt harum. Eos delectus at quae?"
        }
      ]
    };
  },

  computed: {
    post() {
      return this.posts.find(post => post.id === this.id);
    }
  }
};
</script>

