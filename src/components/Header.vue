<template>
  <div class="my-w-80">
    <div class="header-content">
      <div>
        <img src="../assets/img/dc-logo.png" alt="logo" />
      </div>
      <nav>
        <ul class="my-nav-header">
          <li v-for="(element, index) in navHeder" :key="index">
            <a :href="element.url">{{ element.text }}</a>
          </li>
        </ul>
      </nav>
    </div>
  </div>
</template>

<script>
export default {
  name: "HomeHeader",
  data: function () {
    return {
      navHeder: [
        {
          text: "charactecrs",
          url: "#",
          current: true,
        },
        {
          text: "comics",
          url: "#",
          current: false,
        },
        {
          text: "movies",
          url: "#",
          current: false,
        },
        {
          text: "tv",
          url: "#",
          current: false,
        },
        {
          text: "games",
          url: "#",
          current: false,
        },
        {
          text: "collectivles",
          url: "#",
          current: false,
        },
        {
          text: "videos",
          url: "#",
          current: false,
        },
        {
          text: "fans",
          url: "#",
          current: false,
        },

        {
          text: "news",
          url: "#",
          current: false,
        },
        {
          text: "shop",
          url: "#",
          current: false,
        },
      ],
    };
  },
};
</script>

<style  lang="scss" scoped>
div.my-w-80 {
  width: 70%;
  margin: 0 auto;
}
div.header-content {
  height: 100px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem;
  div {
    border: 1px solid black;
  }
}
/* .active {
  content: "";
  display: block;
  height: 3px;
  width: 100%;
  background-color: RGB(2, 130, 249);
  position: absolute;
  bottom: 0;
  left: 0;
} */
ul.my-nav-header {
  display: flex;
  align-items: center;
  height: 100px;
  /*  border: 1px solid black; */

  li {
    height: 100px;

    line-height: 100px;
    list-style-type: none;
    margin-left: 1rem;
    position: relative;
    /*  border-bottom: 3px solid RGB(2, 130, 249); */

    a {
      text-decoration: none;
      text-transform: uppercase;
      color: black;
    }
    :hover {
      color: RGB(2, 130, 249);
    }
  }
}
li:active {
  border-bottom: 3px solid RGB(2, 130, 249);
}
</style>