<script >
import AppHeader from './components/AppHeader.vue';



export default {
  data() {
    return {};
  },
  components: { AppHeader },
}
</script>

<template>
<AppHeader />
</template>

<style lang="scss">
@use "./style/general.scss" as *;
@use "style/partials/variable" as *;
@import '@fortawesome/fontawesome-free/css/all.css';
</style>
