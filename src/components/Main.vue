<template>
  <div class="main-container">
    <div class="main-content-top">
      <section>
        <h5>Content</h5>
      </section>
    </div>
    <div class="main-content-bottom">
      <nav>
        <section class="nav-buy">
          <div>
            <img src="../assets/img/buy-comics-digital-comics.png" alt="" />
          </div>
          <a href="#">digital</a>
        </section>
        <section class="nav-buy">
          <div>
            <img src="../assets/img/buy-comics-merchandise.png" alt="" />
          </div>
          <a href="#">digital</a>
        </section>
        <section class="nav-buy">
          <div>
            <img src="../assets/img/buy-comics-subscriptions.png" alt="" />
          </div>
          <a href="#">digital</a>
        </section>
        <section class="nav-buy">
          <div>
            <img src="../assets/img/buy-comics-shop-locator.png" alt="" />
          </div>
          <a href="#">digital</a>
        </section>
        <section class="nav-buy">
          <div>
            <img src="../assets/img/buy-dc-power-visa.svg" alt="" />
          </div>
          <a href="#">digital</a>
        </section>
      </nav>
    </div>
  </div>
</template>

<script>
export default {
  name: "HomeMain",
  /* data: function () {
    return {
      navbuyComics: [
        {
          text: "dicital comics",
          url: "#",
          current: true,
          src: "buy-comics-digital-comics.png",
        },
        {
          text: "dc merchandice",
          url: "#",
          current: false,
          src: "buy-comics-merchandise.png",
        },
        {
          text: "subscription",
          url: "#",
          current: false,
          src: "buy-comics-subscriptions.png",
        },
        {
          text: "comic shop locator",
          url: "#",
          current: false,
          src: "buy-comics-shop-locator.png",
        },
        {
          text: "dc power visa",
          url: "#",
          current: false,
          src: "buy-dc-power-visa.svg",
        },
      ],
    };
  }, */
};
</script>

<style  lang="scss" scoped>
.main-container {
  color: RGB(255, 255, 255);
}

.main-content-top {
  height: 150px;
  background-color: RGB(28, 28, 28);
  section {
    width: 70%;
    margin: 0 auto;

    h5 {
      line-height: 150px;
    }
  }
}
.main-content-bottom {
  height: 180px;
  background-color: RGB(2, 130, 249);
  nav {
    display: flex;
    align-items: center;
    justify-content: space-between;
    width: 70%;
    margin: 0 auto;
    height: 100%;
    section {
      display: flex;
      align-items: center;
      a {
        text-decoration: none;
        color: white;
      }

      div {
        width: 120px;
        height: 120px;

        margin-left: 1rem;

        img {
          width: 100%;
          object-fit: contain;
          max-height: 100%;
          cursor: pointer;
        }
      }
    }
  }
}
.nav-buy {
  display: flex;
}

/* ul {
  display: flex;
  justify-content: space-between;

  li {
    display: flex;
    align-items: center;

    padding: 0 2.5rem;
    border: 1px solid white;
    width: calc(100% / 5);
    div {
      width: 80%;
      height: 80%;
      background-color: bisque;
    }
  }
  a {
    text-decoration: none;
    padding: 0 0.5rem;
    color: RGB(255, 255, 255);

    img {
      width: 100%;
      object-fit: cover;
      height: 100%;
    }
  }
} */
</style>