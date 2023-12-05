<script>
export default {
  data() {
    return {

    }
  }
}
</script>

<template>
  <div class="jumbo">
    <div class="jumbo-content">
      <p>MOVING WITHOUT THE HASSLE</p>
      <h1>WE MAKE IT SIMPLE</h1>
      <p>PROFESSIONAL SERVICE WITH QUALITY AND CUSTOMERS SATISFACTION</p>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "../style/partials/variable" as *;
.jumbo {
  width: 100%;
  height: 450px;
  background-image: url(../assets/img/avada-movers-homeherobackground-final.jpg);
  background-position: top;
  background-size: cover;

  .jumbo-content {
    width: 100%;
    height: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;

    h1{
      padding: 1.2rem 0;
      font-size: 2.8rem;
    }

    p {
      font-size: .8rem;
      font-weight: bold;
      color: $secondary-text;
    }
  }
}
</style>