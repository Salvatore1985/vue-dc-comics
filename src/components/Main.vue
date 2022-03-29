<template>
  <div class="main-container">
    <Jumbotron />
    <div class="main-content-top">
      <section>
        <h5>Content</h5>
      </section>
    </div>
    <div class="main-content-bottom">
      <nav>
        <!--         aquisti -->
        <section
          class="nav-buy"
          v-for="(element, index) in navbuyComics"
          :key="index"
        >
          <div>
            <img
              :src="require(`@/assets/img/${element.src}`)"
              :alt="element.text"
            />
          </div>
          <a :href="element.url">{{ element.text }}</a>
        </section>
      </nav>
    </div>
  </div>
</template>

<script>
import Jumbotron from "./Jumbotron.vue";
export default {
  name: "HomeMain",
  components: {
    Jumbotron,
  },
  data: function () {
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
      listThumb: [
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
          price: "$19.99",
          series: "Action Comics",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
          price: "$3.99",
          series: "American Vampire 1976",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
          price: "$16.99",
          series: "Aquaman",
          type: "graphic novel",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
          price: "$2.99",
          series: "Batgirl",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          price: "$3.99",
          series: "Batman",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          price: "$2.99",
          series: "Batman Beyond",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
          price: "$3.99",
          series: "Batman/Superman",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
          price: "$4.99",
          series: "Batman/Superman Annual",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
          price: "$5.99",
          series: "Batman: The Joker War Zone",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
          price: "$6.99",
          series: "Batman: Three Jokers",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
          price: "$4.99",
          series: "Batman: White Knight Presents: Harley Quinn",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
          price: "$16.99",
          series: "Catwoman",
          type: "graphic novel",
        },
      ],
    };
  },
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
  height: 150px;
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
        width: 80px;
        height: 80px;

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
</style>