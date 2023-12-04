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
  <div class="container">
    <div class="row">
      <div class="col">
        <i class="fa-solid fa-phone-flip"></i>
        <span>Call us for a Free quote: 1.800.555.6789</span>
      </div>
      <div class="col">
        <ul>
          <li>
            <a href=""><i class="fa-brands fa-facebook-f"></i></a>
          </li>
          <li>
            <a href=""><i class="fa-brands fa-twitter"></i></a>
          </li>
          <li>
            <a href=""><i class="fa-brands fa-instagram"></i></a>
          </li>
          <li>
            <a href=""><i class="fa-brands fa-youtube"></i></a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</div>
</template>

<style lang="scss" scoped>
@use "../style/partials/variable" as *;

.wrap {
  background-color: $header-top-bg;
  color: white;

  .container {
    max-width: 70%;
    margin: 0 auto;
    height: 50px;

    .row {
      display: flex;
      justify-content: space-between;
      align-items: center;
      height: 100%;

      .col {

        ul {
          display: flex;
          list-style-type: none;

          li {
            font-size: 1.2rem;
            padding-left: 1rem;
            a{
              color: inherit;

            }
          }
        }

        span {
          padding-left: 1rem;
        }
      }
    }
  }
}
</style>