<script>
export default {
  data() {
    return {}
  },
  props: {
    testimonial: Object,
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
      <img :src="getImageUrl(testimonial.img)" alt="">
    </div>

    <div class="card-content">
      <h3>{{ testimonial.title }}</h3>
      <p>{{ testimonial.content }}</p>
    </div>
  </div>

</template>

<style lang="scss" scoped>
@use "../style/partials/variable" as *;
.card {
  text-align: center;
  .card-img {
    width: 150px;
    margin: 0 auto;


    img {
      border-radius: 50%;
    }
  }

  .card-content {
    padding: 3rem 0;

    h3 {
      color: $btn-bg;
      font-size: 2rem;
      padding-bottom: 3rem;
    }

    p {
      color: $secondary-text;
      font-size: .9rem;
      line-height: 1.5rem;
    }
  }
}
</style>