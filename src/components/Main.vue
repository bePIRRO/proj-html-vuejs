<template>
  <main>
    <div v-for="card in cards" :key="card">
      <Card />
    </div>

    <div>
      <TopButton />
    </div>
  </main>
</template>

<script>
import Card from "./Card.vue";
import TopButton from "./TopButton.vue";

export default {
  name: "Main",
  components: {
    Card,
    TopButton,
  },
  props: {},
};
</script>

<style scoped>
@import "../assets/scss/_generics.scss";
</style>
