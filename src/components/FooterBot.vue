<template>
  <div class="wrapped-social">
    <button>Sign-up now!</button>
    <ul>
      <li><a href="#">follower us</a></li>
      <li>
        <!--  <a href="#"> <img src="" alt="" /></a> -->
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "FooterDcComicsBot",
  data() {
    return [
      {
        icons: "footer-facebook.png",
      },
    ];
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
  ul {
    list-style-type: none;
  }
}
</style>