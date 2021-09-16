<template>
  <div class="card-container">
    <a :href="card.link">
      <div class="my-5 card">
        <img :src="getImg(card.url)" alt="img" class="m-5" />
        <h3 class="mb-5">{{ card.text }}</h3>
      </div>
    </a>
  </div>
</template>

<script>
export default {
  name: "Card",

  props: ["card"],
  methods: {
    getImg() {
      return require(`@/assets/img/${this.card.url}`);
    },
  },
};
</script>

<style scoped lang="scss">
@import "@/assets/scss/_generics.scss";
@import "@/assets/scss/_card.scss";
</style>
