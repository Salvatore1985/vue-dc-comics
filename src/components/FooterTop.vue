<template>
  <div class="wrapped-link">
    <div>
      <h5>dc comics</h5>
      <ul>
        <li>
          <a href="#">characters</a>
        </li>
        <li>
          <a href="#">comics</a>
        </li>
        <li>
          <a href="#">movies</a>
        </li>
        <li>
          <a href="#">tv</a>
        </li>
        <li>
          <a href="#">games</a>
        </li>
        <li>
          <a href="#">videos</a>
        </li>
        <li>
          <a href="#">news</a>
        </li>
      </ul>
      <h5>dc comics</h5>
      <ul>
        <li><a href="#">shop DC</a></li>
        <li><a href="#">shop DC collectibles</a></li>
      </ul>
    </div>
    <div>
      <h5>dc comics</h5>
      <ul>
        <li><a href="#">terms of use</a></li>
        <li><a href="#">privacy policy (new)</a></li>
        <li><a href="#">ad choices</a></li>
        <li><a href="#">advertising</a></li>
        <li><a href="#">jobs</a></li>
        <li><a href="#">subscriptions</a></li>
        <li><a href="#">talent workshops</a></li>
        <li><a href="#">CPSC certificates</a></li>
        <li><a href="#">shop help</a></li>
        <li><a href="#">contact us</a></li>
      </ul>
    </div>
    <div>
      <h5>dc comics</h5>
      <ul>
        <li><a href="#">dC</a></li>
        <li><a href="#">MAD magazine</a></li>
        <li><a href="#">dC kids</a></li>
        <li><a href="#">dC universe</a></li>
        <li><a href="#">dC power visa</a></li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "FooterDcComics",
  props: ["dcComicsLInk"],
};
</script>

<style  lang="scss" scoped>
@import "../assets/scss/style.scss";

.wrapped-link {
  display: flex;
}
div {
  padding: 1rem;
  h5 {
    text-transform: uppercase;
    color: white;
    padding: 1rem 0;
  }
  ul {
    list-style-type: none;
    li {
      padding: 0.3rem 0;
      a {
        text-transform: capitalize;
        color: #747373;
        font-size: 0.8rem;
      }
    }
  }
}
</style>