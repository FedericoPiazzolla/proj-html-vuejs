<script>
import MainBigBtn from './MainBigBtn.vue';
import MainTestimonialsSection from './MainTestimonialsSection.vue';

export default {
  data() {
      return {};
  },
  components: { MainBigBtn, MainTestimonialsSection },
}
</script>

<template>
  <MainBigBtn />
  <MainTestimonialsSection />
</template>

<style lang="scss" scoped>
@use "../style/partials/variable" as *;
</style>