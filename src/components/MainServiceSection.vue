<script>
export default {
  data() {
    return {

    }
  }
}
</script>

<template>
<div class="container">
  <div class="card-title">
    <h3>WE ARE PROFESSIONAL</h3>
    <h2>Full-Service Solution</h2>
  </div>
  <div class="row">
    <div class="col">

    </div>
  </div>
</div>
</template>

<style lang="scss" scoped>
@use "../style/partials/variable" as *;
.container {
  width: 80%;
  margin: 0 auto;
  padding: 4rem 0;

  .card-title {
    text-align: center;

    h3{
      color: $secondary-text;
      font-size: .9rem;
      padding-bottom: 1rem;
    }

    h2 {
      color: $lime-text;
      font-size: 2.8rem;
    }
  }

  .row {
    display: flex;

    .col {
      width: calc(100% / 3);
    }
  }
}
</style>