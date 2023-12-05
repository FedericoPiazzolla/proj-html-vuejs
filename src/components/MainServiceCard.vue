<script>
export default {
  data() {
    return {
      
    }
  },
  props: {
    card: Object,
  },
  methods: {
    getImageUrl(imgName) {
      return new URL(`../assets/img/${imgName}`, import.meta.url).href;
    },
  }
}
</script>

<template>
<div class="card">
  <div class="card-img">
    <img :src="getImageUrl(card.imgPath)" alt="">
  </div>

  <div class="card-content">
    <h3>{{ card.title }}</h3>
    <p>{{ card.content }}</p>
    <a href="">{{ card.contentBtn }}</a>
  </div>
</div>
</template>

<style lang="scss" scoped>
@use "../style/partials/variable" as *;

.card {
  background-color: $section-light-bg;
  padding: 1rem;
  text-align: center;

  .card-img {
    overflow: hidden;
    img {
      margin-bottom: 1rem;
      transition: transform 0.5s ease-in-out;
      transform-origin: center center;

      &:hover {
        transform: scale(1.1);
      }
    }
  }

  .card-content {
    background-color: white;
    padding: 1rem;
    padding-bottom: 3rem;

    h3 {
      color: $btn-bg;
      padding-bottom: 1rem;
      font-size: 1.5rem;
    }

    p {
      font-size: .9rem;
      color: $secondary-text;
      padding-bottom: 2.5rem;
    }

    a {
      color: white;
      text-decoration: none;
      background-color: $btn-bg;
      padding: .8rem 1.4rem;
      border-radius: 2rem;

      &:hover {
        background-color: lighten($btn-bg, 15%);
      }
      
    }
  }
}
</style>