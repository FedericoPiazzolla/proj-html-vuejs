<script>
import MainServiceCard from "./MainServiceCard.vue";

export default {
  data() {
    return {
      serviceElem: [
        {
          imgPath: "avada-movers-serviceonephoto-final-400x255.jpg",
          title: "Two Man Teams",
          content:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Consectetur maiores repellendus libero enim, facilis modi error aliquid est, eum sint consequuntur animi dicta temporibus similique laudantium, ab laborum sit pariatur!",
          contentBtn: "READ MORE",
        },
        {
          imgPath: "avada-movers-servicetwophoto-final-400x255.jpg",
          title: "We Do All The Lifting",
          content:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Consectetur maiores repellendus libero enim, facilis modi error aliquid est, eum sint consequuntur animi dicta temporibus similique laudantium, ab laborum sit pariatur!",
          contentBtn: "READ MORE",
        },
        {
          imgPath: "avada-movers-servicethreephoto-final-400x255.jpg",
          title: "Two Man Teams",
          content:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Consectetur maiores repellendus libero enim, facilis modi error aliquid est, eum sint consequuntur animi dicta temporibus similique laudantium, ab laborum sit pariatur!",
          contentBtn: "READ MORE",
        },
      ],
    };
  },
  components: { MainServiceCard },
};
</script>

<template>
  <div class="container">
    <div class="card-title">
      <h3>WE ARE PROFESSIONAL</h3>
      <h2>Full-Service Solution</h2>
    </div>
    <div class="row">
      <div class="col" v-for="item in serviceElem">
        <MainServiceCard :card="item" />
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "../style/partials/variable" as *;
.container {
  width: 80%;
  max-width: 1100px;
  margin: 0 auto;
  padding: 4rem 0;

  .card-title {
    text-align: center;

    h3 {
      color: $secondary-text;
      font-size: 0.9rem;
      padding-bottom: 1rem;
    }

    h2 {
      color: $lime-text;
      font-size: 2.8rem;
    }
  }

  .row {
    display: flex;
    justify-content: space-between;
    gap: 1.5rem;
    padding: 2rem 0;

    .col {
      width: calc(100% / 3 - 1.5rem);
    }
  }
}
</style>
