<script>
import HeaderTop from './HeaderTop.vue';

export default {
    data() {
        return {};
    },
    components: { HeaderTop }
}
</script>

<template>
  <div class="container">
    <HeaderTop />
  </div>
</template>

<style lang="scss" scoped>
.container {
  max-width: 70%;
  margin: 0 auto;

}
</style>