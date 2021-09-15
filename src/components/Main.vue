<template>
  <main>
    <div v-for="card in cards" :key="card">
      <Card />
    </div>
  </main>
</template>

<script>
import Card from "./Card.vue";

export default {
  name: "Main",
  components: {
    Card,
  },
  props: {},
};
</script>

<style scoped></style>
