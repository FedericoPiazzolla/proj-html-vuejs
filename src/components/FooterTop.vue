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
  },
};
</script>

<template>
  <footer>
    <div class="container">
      <div class="row">
        <div class="col">
          <h3>{{ leftCol.title }}</h3>

          <p>{{ leftCol.content }}</p>
          <img :src="getImageUrl(leftCol.imgPath)" alt="" />
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
    </div>
  </footer>
</template>

<style lang="scss" scoped>
@use "../style/partials/variable" as *;
footer {
  margin-bottom: 2rem;

  .container {
    width: 100%;
    display: flex;
    justify-content: center;
    background-color: white;
  }

  .row {
    display: flex;
    width: 80%;
    padding: 2.5rem 0;
    background-color: white;

    .col {
      width: calc(100% / 3);
      padding: 1rem;

      h3 {
        color: $primary-text;
        padding-bottom: 1.5rem;
      }

      p {
        color: $secondary-text;
        line-height: 1.5rem;
        font-size: 0.9rem;
      }

      img {
        padding: 3rem 0;
      }

      ul {
        list-style-type: none;

        li {
          padding-bottom: 1.6rem;
          color: $secondary-text;
          font-weight: 500;

          a {
            color: inherit;
            text-decoration: none;

            &:hover {
              color: $lime-text;
            }
          }
        }
      }
    }
  }
}
</style>
