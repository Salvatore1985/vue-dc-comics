<template>
  <div class="wrapped-link">
    <div>
      <ul>
        <li>
          <a href="#">{{ dcComicsLInk }}</a>
        </li>
      </ul>
      <!-- <h5>dc comics</h5>
      <ul>
        <li><a href="#">link</a></li>
        <li><a href="#">link</a></li>
        <li><a href="#">link</a></li>
        <li><a href="#">link</a></li>
        <li><a href="#">link</a></li>
        <li><a href="#">link</a></li>
      </ul> -->
    </div>
    <!--  <div>
      <h5>dc comics</h5>
      <ul>
        <li><a href="#">link</a></li>
      </ul>
    </div>
    <div>
      <h5>dc comics</h5>
      <ul>
        <li><a href="#">privacy policy (new)</a></li>
        <li><a href="#">CPSC certificates</a></li>
        <li><a href="#">link</a></li>
        <li><a href="#">link</a></li>
        <li><a href="#">link</a></li>
        <li><a href="#">link</a></li>
      </ul>
    </div> -->
  </div>
</template>

<script>
export default {
  name: "HomeFooterTop",
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
      }
    }
  }
}
</style>