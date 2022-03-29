<template>
  <div class="my-w-70">
    <div class="header-content">
      <div id="logo">
        <img src="../assets/img/dc-logo.png" alt="logo" />
      </div>
      <nav>
        <ul class="my-nav-header">
          <li
            v-for="(element, index) in navHeder"
            :key="index"
            :class="{ active: element.current }"
          >
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
div.my-w-70 {
  width: 70%;
  margin: 0 auto;
}
div.header-content {
  height: 100px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.my-nav-header {
  display: flex;
  align-items: center;
  height: 100px;

  li {
    /* height: 100px; */

    line-height: 100px;
    list-style-type: none;
    margin-left: 1.5rem;
    position: relative;

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
  border-bottom: 5px solid RGB(2, 130, 249);
}
#logo img {
  width: 80%;
}
</style>