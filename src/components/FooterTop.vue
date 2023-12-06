<script>
export default {
  props: {
    leftCol: Object,
    centralCol: Object,
    rightCol: Object,
  },
  methods: {
    getImageUrl(imgName) {
      return new URL(`../assets/img/${imgName}`, import.meta.url).href;
    },
  }
}
</script>

<template>
  <footer>
    <div class="row">

      <div class="col">
        <h3>{{ leftCol.title }}</h3>

        <p>{{ leftCol.content }}</p>
        <img :src="getImageUrl( leftCol.imgPath )" alt="">
      </div>

      <div class="col">
        <h3>{{ centralCol.title }}</h3>

        <ul>
          <li v-for="(item, index) in centralCol.listItem" :key="index">
            <a href="">{{ item }}</a>
          </li>
        </ul>
      </div>

      <div class="col">
        <h3>{{ rightCol.title }}</h3>

        <ul>
          <li v-for="(item, index) in rightCol.listItem">
            <a href="">
              <i class="fa-solid fa-angle-right"></i>
              {{ item }}
            </a>
          </li>
        </ul>
      </div>
    </div>

  </footer>
</template>

<style lang="scss" scoped>
@use "../style/partials/variable" as *;
footer {
  margin-bottom: 2rem;

  .row {
    display: flex;
    padding: 1rem;
    background-color: white;

    .col {
      width: calc(100% / 3);
      padding: 1rem;

      h3 {

      }
    }
  }
}
</style>