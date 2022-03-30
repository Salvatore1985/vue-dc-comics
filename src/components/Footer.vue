<template>
  <div>
    <div class="footer-top">
      <section class="my-container">
        <section>
          <FooterTop />
        </section>
        <div id="logo">
          <img src="../assets/img/dc-logo-bg.png" alt="" />
        </div>
      </section>
    </div>
    <div class="footer-bottom">
      <section class="my-container">
        <FooterBot />
      </section>
    </div>
  </div>
</template>

<script>
import FooterTop from "./FooterTop.vue";
import FooterBot from "./FooterBot.vue";
export default {
  name: "HomeFooter",
  components: {
    FooterTop,
    FooterBot,
  },
  data() {
    return {
      dcComicsList: [
        "characters",
        "comics",
        "movies",
        "tv",
        "games",
        "videos",
        "news",
      ],
      shopList: ["shop DC", "shop DC collectibles"],
      dcList: [
        "terms of use",
        "privacy policy (new)",
        "ad choices",
        "advertising",
        "jobs",
        "subscriptions",
        "talent workshops",
        "CPSC certificates",
        "ratings",
        "shop help",
        "contact us",
      ],
      sitesList: [
        "dC",
        "MAD magazine",
        "dC kids",
        "dC universe",
        "dC power visa",
      ],
    };
  },
};
</script>

<style  lang="scss" scoped>
@import "../assets/scss/style.scss";
.footer-top {
  background-image: url(../assets/img/footer-bg.jpg);
  background-size: cover;
  height: 500px;
}
.footer-top section.my-container {
  display: flex;
  justify-content: space-between;
}
div#logo {
  height: 500px;

  img {
    width: 120%;
    height: 100%;
    object-fit: cover;
    object-position: center;
  }
}

.footer-bottom {
  background-color: $brand_secondary;
}
</style>