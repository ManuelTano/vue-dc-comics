<template>
  <header>
    <div class="container">
      <nav>
        <div class="image">
          <img src="../assets/img/dc-logo.png" alt="dc-logo" />
        </div>
        <ul>
          <li
            v-for="(link, i) in links"
            :key="i"
            :class="{ active: link.current }"
          >
            <a :href="link.url">{{ link.text }}</a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "MyHeader",
  data() {
    return {
      links: [
        {
          text: "Characters",
          url: "#",
          current: false,
        },
        {
          text: "Comics",
          url: "#",
          current: true,
        },
        {
          text: "Movies",
          url: "#",
          current: false,
        },
        {
          text: "TV",
          url: "#",
          current: false,
        },
        {
          text: "Games",
          url: "#",
          current: false,
        },
        {
          text: "Collectibles",
          url: "#",
          current: false,
        },
        {
          text: "Videos",
          url: "#",
          current: false,
        },
        {
          text: "Fans",
          url: "#",
          current: false,
        },
        {
          text: "News",
          url: "#",
          current: false,
        },
        {
          text: "Shop",
          url: "#",
          current: false,
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "../assets/sass/vars";

header {
  background-color: $white;
  max-height: 140px;
}

nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 15px;
}

ul {
  display: flex;
  align-items: center;

  li {
    height: 100%;
    font-weight: bold;
    display: flex;
    align-items: center;
    cursor: pointer;
  }
}

a {
  color: $gray;
  padding: 0px 10px;
  text-decoration: none;

  &:hover {
    color: $blue;
    border-bottom: 3px solid $blue;
  }
}
</style>