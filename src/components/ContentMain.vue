<template>
  <!-- <div class="my-container"> -->
  <div class="cover">
    <a href="#">
      <img :src="CoverThumb" :alt="CoverType" />
      <h5>{{ CoverType }}</h5>
    </a>
  </div>
  <!-- </div> -->
</template>

<script>
export default {
  name: "ContentMainCards",

  props: ["CoverThumb", "CoverPrice", "CoverSeries", "CoverType"],
};
</script>

<style  lang="scss" scoped>
@import "../assets/scss/style.scss";
/* div.my-container {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
} */
div.cover {
  text-transform: uppercase;
  margin-top: 2rem;
  padding: 1rem;
  a {
    img {
      width: 180px;
      height: 180px;
      object-fit: cover;
      object-position: top;
    }
    h5 {
      padding: 1rem 0;
    }
  }
}
</style>