<script>
import MainBigBtn from './MainBigBtn.vue';
import MainServiceSection from './MainServiceSection.vue';
import MainTestimonialsSection from './MainTestimonialsSection.vue';

export default {
  data() {
      return {};
  },
  components: { MainBigBtn, MainTestimonialsSection, MainServiceSection },
}
</script>

<template>
  <MainBigBtn />
  <MainTestimonialsSection />
  <MainServiceSection />
</template>

<style lang="scss" scoped>
@use "../style/partials/variable" as *;
</style>