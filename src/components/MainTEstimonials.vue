<script>
import TestimonialsCard from "./TestimonialsCard.vue";

export default {
  data() {
    return {
      testimonialsElem: [
        {
          img: "avada-movers-johndoe-final.jpg",
          title: "John Doe",
          content:
          `"Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolore enim sapiente praesentium debitis, magnam culpa harum officia aliquam in quisquam. Nam velit expedita impedit! Cumque officia similique animi vel perspiciatis!"`,
        },
        {
          img: "avada-movers-janedoe-final.jpg",
          title: "Jane Doe",
          content:
            `"Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolore enim sapiente praesentium debitis, magnam culpa harum officia aliquam in quisquam. Nam velit expedita impedit! Cumque officia similique animi vel perspiciatis!"`,
        },
        {
          img: "avada-movers-johnsmith-final.jpg",
          title: "John Smith",
          content:
          `"Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolore enim sapiente praesentium debitis, magnam culpa harum officia aliquam in quisquam. Nam velit expedita impedit! Cumque officia similique animi vel perspiciatis!"`,
        },
      ],
    };
  },
  components: { TestimonialsCard },
};
</script>

<template>
  <div class="wrapper">
    <div class="container">
      <div class="title">
        <h3>HAPPY CUSTOMERS</h3>
        <h2>Testimonials</h2>
      </div>

      <div class="row">
        <div class="col" v-for="card in testimonialsElem">
          <TestimonialsCard :testimonial="card"/>
        </div>
      </div>

      <div class="btn">
        <a href="">READ MORE TESTIMONIALS</a>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "../style/partials/variable" as *;
.wrapper {
  background-image: url("../assets/img/avada-movers-testimonial-background.jpg");
  min-height: 550px;
  background-position: center top;
  background-size: cover;

  .container {
    width: 70%;
    max-width: 1100px;
    margin: 0 auto;

    .title {
      text-align: center;
      padding: 4rem 0;

      h3 {
        color: $secondary-text;
        font-size: 1rem;
      }

      h2 {
        color: $lime-text;
        font-size: 3rem;
        padding: 1.5rem 0;
      }
    }

    .row {
      display: flex;
      justify-content: space-between;
      gap: 1rem;
      padding-bottom: 4rem;

      .col {
        width: calc(100% / 3 - 1rem);
      }
    }

    .btn {
      text-align: center;
      padding: 1rem 0 6rem;

      a {
        color: white;
        text-decoration: none;
        background-color: $btn-bg;
        padding: .8rem 1.4rem;
        border-radius: 2rem;
        font-weight: bold;

        &:hover {
          background-color: lighten($btn-bg, 15%);
        }
      }
    }
  }
}
</style>
