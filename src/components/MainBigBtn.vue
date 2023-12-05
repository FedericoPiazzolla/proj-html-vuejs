<script>
export default {
  data() {
    return{}
  }
}
</script>

<template>
<div class="wrap">
  <a href="">
    <i class="fa-regular fa-paper-plane"></i>
    <span>GET A FREE QUOTE ONLINE NOW!</span>
  </a>
</div>
</template>

<style lang="scss" scoped>
@use "../style/partials/variable" as *;
.wrap {
  width: 100%;
  height: 100px;
  a {
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    color: white;
    text-decoration: none;
    background-color: $btn-bg;

    span {
      padding-left: 1rem;
    }

    &:hover {
      background-color: lighten(($btn-bg),  15%);
    }
  }
}
</style>