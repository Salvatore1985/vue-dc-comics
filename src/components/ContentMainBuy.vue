<template>
  <!-- <div class="my-container"> -->
  <div class="cover">
    <a :href="CoverBuyUrl">
      <div>
        <img
          :src="require(`@/assets/img/${CoverBuySrc}`)"
          :alt="CoverBuyText"
        />
        <span>{{ CoverBuyText }}</span>
      </div>
    </a>
  </div>
  <!-- </div> -->
</template>

<script>
export default {
  name: "ContentMainBuyCards",

  props: ["CoverBuyText", "CoverBuyUrl", "CoverBuyCurrent", "CoverBuySrc"],
};
</script>

<style  lang="scss" scoped>
@import "../assets/scss/style.scss";

div.cover {
  text-transform: uppercase;
  padding: 2rem 1rem;
  a {
    div {
      display: flex;
      justify-content: center;
      align-items: center;
      img {
        width: 50px;
        height: 50px;
        object-fit: contain;
      }
    }
    span {
      padding: 0 1rem;
      font-size: 0.8rem;
    }
  }
}
</style>