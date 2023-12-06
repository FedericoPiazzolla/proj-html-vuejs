<script>
export default {
  data() {
    return {

    }
  }
}
</script>

<template>
  <div class="wrap">
    <div class="row">
      <div class="col">
        <p class="subtitle">HEADACHE FREE</p>
        <h2>
          Award Winning 
          <br>
          Moving Company
        </h2>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Fuga, velit molestiae. Omnis cumque eligendi, dolore facere placeat laudantium possimus doloremque deserunt eum sint rem quisquam saepe vitae illum, esse repellat.
        </p>
        <a href="">READ OUR TESTIMONIALS</a>
      </div>
      
    </div>
  </div>
</template>

<style lang="scss" scoped> 
@use "../style/partials/variable" as *;
.wrap {
  background-color: $section-light-bg;
  padding: 6.2rem 0;
  min-height: 600px;
  .row {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;

    .col {
      width: 70%;
      max-width: 1100px;
      text-align: center;

      h2 {
        color: $lime-text;
        font-size: 2.8rem;
      }

      p {
        padding: 2.4rem 0;
        color: $secondary-text;

        &.subtitle {
          font-weight: bolder;
        }
      }

      a {
        color: white;
        text-decoration: none;
        background-color: $btn-bg;
        padding: .8rem 3rem;
        border-radius: 2rem;

        &:hover {
          background-color: lighten(($btn-bg),  15%);
        }
      }
    }
  }
}
</style>