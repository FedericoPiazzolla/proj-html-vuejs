<script>
export default {
  data() {
    return {
      boxContent: {
        subTitle: "WE REMOVE THE HEADACHE FROM MOVING",
        title: "Move With Ease",
        content: "With our super simple service we can take you from getting a quote, right through to being in your new home with all of your belongings securely packed and safely delivered, even in the rooms of your choice.",
        boxBtn: "GET A FREE QUOTE NOW",
      },
    }
  }
}
</script>

<template>
  <section class="bg-section">
    <div class="container">
     <div class="box">
        <h3>{{ boxContent.subTitle }}</h3>
        <h2>{{ boxContent.title }}</h2>
        <hr>
        <p>{{ boxContent.content }}</p>
        <a href="">{{ boxContent.boxBtn }}</a>
      </div> 
    </div>
    
  </section>
</template>

<style lang="scss" scoped>
@use "../style/partials/variable" as *;
.bg-section {
  background-image: url("../assets/img/avada-movers-movewithease-background-new.jpg");
  background-size: cover;
  background-position: center top;

  .container {
    width: 70%;
    max-width: 1100px;
    margin: 0 auto;
    min-height: 600px;
    display: flex;
    flex-direction: row-reverse;
    align-items: center;
    .box {
      width: 55%;
      text-align: center;
      background-color: $header-top-bg;
      border: 15px solid $border-dark-green;
      padding: 3rem 1.5rem;
      color: white;

      h3 {
        font-size: .8rem;
        padding-bottom: 2rem;
      }

      h2 {
        font-size: 2.5rem;
        padding-bottom: 2rem;
      }

      hr {
        border: 1px solid white;
        width: 70%;
        margin: 0 auto;
      }

      p {
        font-size: 1rem;
        padding: 3rem 0;
        line-height: 2rem;
      }

      a {
        text-decoration: none;
        color: inherit;
        background-color: $btn-bg;
        padding: .8rem 1.2rem;
        border-radius: 2rem;
        font-weight: bold;

        &:hover {
          background-color: lighten($btn-bg, 15);
        }
      }
    }
  }
}
</style>