<template>
  <div>
    <div class="footer-top">
      <section class="my-container">
        <FooterTop />
      </section>
    </div>
    <div class="footer-bottom"></div>
  </div>
</template>

<script>
import FooterTop from "./FooterTop.vue";
export default {
  name: "HomeFooter",
  components: {
    FooterTop,
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
.footer-top {
  background-image: url(../assets/img/footer-bg.jpg);
  background-size: cover;
}
</style>