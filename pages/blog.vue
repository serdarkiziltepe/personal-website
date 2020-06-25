<template>
  <div class="container">
    <!-- <Header /> -->
    <div class="blog">
      <article>
        <h1>Neomorphic Design</h1>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quibusdam, facere. Harum cupiditate accusantium omnis consequatur. Facilis expedita illum quibusdam repellat debitis a suscipit aliquid nesciunt harum. Eos delectus at quae?</p>
      </article>

      <article>
        <h1>Neomorphic Design</h1>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quibusdam, facere. Harum cupiditate accusantium omnis consequatur. Facilis expedita illum quibusdam repellat debitis a suscipit aliquid nesciunt harum. Eos delectus at quae?</p>
      </article>

      <article>
        <h1>Neomorphic Design</h1>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quibusdam, facere. Harum cupiditate accusantium omnis consequatur. Facilis expedita illum quibusdam repellat debitis a suscipit aliquid nesciunt harum. Eos delectus at quae?</p>
      </article>

      <article>
        <h1>Neomorphic Design</h1>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quibusdam, facere. Harum cupiditate accusantium omnis consequatur. Facilis expedita illum quibusdam repellat debitis a suscipit aliquid nesciunt harum. Eos delectus at quae?</p>
      </article>

      <article>
        <h1>Neomorphic Design</h1>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quibusdam, facere. Harum cupiditate accusantium omnis consequatur. Facilis expedita illum quibusdam repellat debitis a suscipit aliquid nesciunt harum. Eos delectus at quae?</p>
      </article>

      <article>
        <h1>Neomorphic Design</h1>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quibusdam, facere. Harum cupiditate accusantium omnis consequatur. Facilis expedita illum quibusdam repellat debitis a suscipit aliquid nesciunt harum. Eos delectus at quae?</p>
      </article>

      <article>
        <h1>Neomorphic Design</h1>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quibusdam, facere. Harum cupiditate accusantium omnis consequatur. Facilis expedita illum quibusdam repellat debitis a suscipit aliquid nesciunt harum. Eos delectus at quae?</p>
      </article>
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

<style lang="scss">
.blog {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 100px;

  article {
    box-shadow: -5px -5px 20px white, 5px 5px 20px #babecc;
    padding: 30px 60px;

    background-color: #ebecf0;

    h1 {
      color: #ae1100;
    }
  }
}
</style>
