<template>
  <div class="wrapped-social">
    <button>Sign-up now!</button>
    <ul>
      <li><a href="#">followe us</a></li>
      <li v-for="(element, index) in iconsList" :key="index">
        <a :href="element.url">
          <img
            :src="require(`@/assets/img/${element.icons}`)"
            :alt="element.alt"
        /></a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "FooterDcComicsBot",
  data() {
    return {
      iconsList: [
        {
          alt: "facebook",
          icons: "footer-facebook.png",
          url: "#",
        },
        {
          alt: "twitter",
          icons: "footer-twitter.png",
          url: "#",
        },
        {
          alt: "youtube",
          icons: "footer-youtube.png",
          url: "#",
        },
        {
          alt: "pinterest",
          icons: "footer-pinterest.png",
          url: "#",
        },
        {
          alt: "periscope",
          icons: "footer-periscope.png",
          url: "#",
        },
      ],
    };
  },
};
</script>

<style  lang="scss" scoped>
@import "../assets/scss/style.scss";

.wrapped-social {
  display: flex;
  align-items: center;
  justify-content: space-between;
  button {
    background-color: $brand_secondary;
    border: 2px solid $brand_primary;
    color: white;
    padding: 0.5rem;
    text-transform: uppercase;
    margin: 1.5rem;
    cursor: pointer;
  }
  li:nth-child(1) {
    a {
      color: $brand_primary;
      font-size: 1.5rem;
      font-weight: bold;
      text-transform: uppercase;
    }
  }
  ul {
    list-style-type: none;
    display: flex;
    align-items: center;
    li {
      padding: 0 0.5rem;
    }
  }
}
</style>