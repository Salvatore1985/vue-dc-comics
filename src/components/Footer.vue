<template>
  <div>
    <div class="footer-top">
      <section></section>
      <section id="position-logo">
        <img class="logo-footer-dc" src="../assets/img/dc-logo-bg.png" alt="" />
      </section>
    </div>
    <div class="footer-bottom">
      <nav class="nav-footer">
        <section>
          <div>
            <button>sign</button>
          </div>
        </section>
        <section>
          <div>
            <ul>
              <li><a href="#"> </a></li>
            </ul>
          </div>
        </section>
      </nav>
    </div>
  </div>
</template>

<script>
export default {
  name: "HomeFooter",
};
</script>

<style  lang="scss" scoped>
.footer-top {
  height: 400px;
  background-image: url("../assets/img/footer-bg.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;

  display: flex;
  section {
    width: 50%;
    height: 100%;
    border: 1px solid white;
  }
}

.footer-bottom {
  display: block;
  height: 100px;
  width: 100%;
  background-color: RGB(48, 48, 48);
  display: flex;
}
.logo-footer-dc {
  position: absolute;
  left: 0px;
  bottom: -100px;
}
#position-logo {
  position: relative;
}

.nav-footer {
  width: 70%;
  margin: 0 auto;
  display: flex;
  section {
    width: 50%;
    height: 100%;
    border: 1px solid white;
  }
}
</style>