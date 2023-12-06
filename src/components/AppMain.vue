<script>
import MainBigBtn from './MainBigBtn.vue';
import MainMWE from './MainMWE.vue';
import MainServiceSection from './MainServiceSection.vue';
import MainTEstimonials from './MainTEstimonials.vue';
import MainTestimonialsSection from './MainTestimonialsSection.vue';

export default {
  data() {
    return {};
  },
  components: { MainBigBtn, MainTestimonialsSection, MainServiceSection, MainMWE, MainTEstimonials },
}
</script>

<template>
  <MainBigBtn />
  <MainTestimonialsSection />
  <MainServiceSection />
  <MainMWE />
  <MainTEstimonials />
</template>

<style lang="scss" scoped>
@use "../style/partials/variable" as *;
</style>