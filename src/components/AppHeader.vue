<script>
import HeaderTop from './HeaderTop.vue';

export default {
    data() {
        return {
          logoSrc: "avada-movers-logo.png",
          menuItems: [
            {label: "Home"},
            {label: "Rates"},
            {label: "Testimonials"},
            {label: "FAQ"},
            {label: "Blog"},
            {label: "Contacts"},
          ],
        };
    },
    components: { HeaderTop },
    methods: {
      getImageUrl(imgName) {
        return new URL(`../assets/img/${imgName}`, import.meta.url).href;
      },
    }
}
</script>

<template>
  <header>
    <div class="container">
      <HeaderTop />
      
      <div class="header-bottom">
        <img :src="getImageUrl(logoSrc)" alt="">

        <nav>
          <ul>
            <li v-for="(item, index) in menuItems" :key="index">
              <a href="" v-if="index < menuItems.length - 1">{{ item.label }}</a>
              <a class="btn" href="" v-else>FREE QUOTE</a>
            </li>
          </ul>
        </nav>
      </div>
      
    </div>
  </header>
  
</template>

<style lang="scss" scoped>
@use "../style/partials/variable" as *;
.header-bottom {
  display: flex;
  justify-content: space-between;
  max-width: 70%;
  margin: 0 auto;
  padding: 1rem 0;
  height: 90px;

  nav {


    ul {
      list-style-type: none;
      display: flex;
      align-items: center;
      height: 100%;

      li {
        padding-left: 1.4rem;

        a {
          color: inherit;
          text-decoration: none;
          font-weight: bolder;

          &.btn {
            background-color: $btn-bg;
            color: white;
            padding: .8rem 1.2rem;
            border-radius: 2rem;
            margin-left: 1.2rem;

            &:hover {
              background-color: lighten(($btn-bg),  15%);
              color: white;
            }
          }

          &:hover {
            color: $header-top-bg;
          }
        }
      }
    }
  }

  
}
</style>