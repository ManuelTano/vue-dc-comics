<template>
  <ul class="card">
    <li v-for="(card, i) in cards" :key="i">
      <a href="#">
        <img :src="card.thumb" :alt="card.series" />
        <h5>{{ card.series }}</h5>
      </a>
    </li>
  </ul>
</template>

<script>
export default {
  name: "MyCards",
  components: {},
  props: {
    cards: Array,
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/sass/vars";

.card {
  display: flex;
  flex-wrap: wrap;
  li {
    width: calc(100% / 6);
  }
}

a {
  text-decoration: none;
  color: white;
}

</style>
