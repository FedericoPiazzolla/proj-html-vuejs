<script>
import FooterTop from "./FooterTop.vue";

export default {
  data() {
    return {
      socialIcons: [
        `fa-facebook-f`,
        `fa-x-twitter`,
        `fa-instagram`,
        `fa-youtube`,
      ],
      LeftCol: {
        title: "ABOUT",
        content:
          "Lorem ipsum dolor sit amet consectetur adipisicing elit. Porro alias in, perspiciatis reprehenderit cupiditate, ut exercitationem reiciendis eos, nostrum distinctio minima deleniti adipisci quo.",
        imgPath: "avada-movers-logo.png",
      },
      centralCol: {
        title: "AVADA MOVERS",
        listItem: ["Home", "Rates", "Testimonials", "Blog", "Free Quote"],
      },
      rightCol: {
        title: "RECENT POSTS",
        listItem: [
          "Heading Out To College?",
          "Moving Your Business?",
          "Outstanding Quality",
          "Cost of Moving",
          "Best Moving Tips",
        ],
      },
    };
  },
  components: { FooterTop },
};
</script>

<template>
  <footer>
    <FooterTop :leftCol="LeftCol" :centralCol="centralCol" :rightCol="rightCol" />

    <div class="container">
      <div class="row">
        <div class="col">
          <p>
            © Copyright 2012 - 2023 | Avada Website Builder by ThemeFusion | All
            Rights Reserved | Powered by WordPress
          </p>
        </div>

        <div class="col-icon">
          <ul>
            <li v-for="icon in socialIcons">
              <a href="">
                <i :class="`fa-brands ${icon}`"></i>
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
  background-color: $header-top-bg;
  padding: .5rem 0 2rem;

  .container {
    width: 60%;
    max-width: 1100px;
    margin: 0 auto;

    .row {
      display: flex;
      flex-direction: column;
      color: white;

      .col {
        p {
          text-align: center;
          font-size: 0.8rem;
        }
      }

      .col-icon {
        padding-top: 1.4rem;
        ul {
          display: flex;
          justify-content: center;
          list-style-type: none;

          li {
            font-size: 1.2rem;
            padding-left: 1rem;
            a {
              color: inherit;

              &:hover {
                color: $primary-text;
              }
            }
          }
        }
      }
    }
  }
}
</style>
