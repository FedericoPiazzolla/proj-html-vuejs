<script>
import MainBigBtn from './MainBigBtn.vue';
import MainMWE from './MainMWE.vue';
import MainServiceSection from './MainServiceSection.vue';
import MainTestimonialsSection from './MainTestimonialsSection.vue';

export default {
  data() {
    return {};
  },
  components: { MainBigBtn, MainTestimonialsSection, MainServiceSection, MainMWE },
}
</script>

<template>
  <MainBigBtn />
  <MainTestimonialsSection />
  <MainServiceSection />
  <MainMWE />
</template>

<style lang="scss" scoped>
@use "../style/partials/variable" as *;
</style>