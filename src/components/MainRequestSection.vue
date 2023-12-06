<script>
export default {
  data() {
    return {

    }
  }
}
</script>

<template>
  <div class="wrapper">
    <div class="container">

      <div class="text-container">
        <h2>Request A Free Quote</h2>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Blanditiis quasi voluptas doloremque similique fugiat. Dolorem neque numquam vitae, assumenda nostrum dolor eius quaerat.</p>
        <a href="">CLICK HERE</a>
      </div>

    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "../style/partials/variable" as *;

.wrapper {
  min-height: 500px;
  background-image: url("../assets/img/avada-movers-request-quote-background.jpg");
  background-size: cover;

  .container {
    width: 50%;
    max-width: 1100px;
    margin: 0 auto;

    .text-container {
      text-align: center;
      padding: 8rem 0;

      h2 {
        color: $lime-text;
        font-size: 2.5rem;
        padding: 2rem 0;
      }

      p {
        font-size: .9rem;
        color: $secondary-text;
        padding-bottom: 4rem;
        line-height: 1.5rem;
      }

      a {
        text-decoration: none;
        color: white;
        background-color: $btn-bg;
        padding: .8rem 1.4rem;
        border-radius: 2rem;
        font-weight: bolder;

        &:hover {
          background-color: lighten($btn-bg, 15%);
        }
      }
    }
  }
}
</style>