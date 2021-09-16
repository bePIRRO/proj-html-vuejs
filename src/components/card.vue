<template>
  <div class="card-container">
    <a :href="card.link">
      <div class="my-5 card">
        <img
          :src="`../assets/images/${this.cards.url}`"
          alt="img"
          class="m-5"
        />
        <h3 class="mb-5">{{ card.text }}</h3>
      </div>
    </a>
  </div>
</template>

<script>
export default {
  name: "Card",
  data() {
    return {
      cards: [
        {
          url: "h5-custom-icon-1.png",
          text: "Languages",
          link: "#",
        },
        {
          url: "h5-custom-icon-2.png",
          text: "Software",
          link: "#",
        },
        {
          url: "h5-custom-icon-3.png",
          text: "Business",
          link: "#",
        },
        {
          url: "h5-custom-icon-4.png",
          text: "Chemistry",
          link: "#",
        },
        {
          url: "h5-custom-icon-5.png",
          text: "Science",
          link: "#",
        },
        {
          url: "h5-custom-icon-6.png",
          text: "DIY%Craft",
          link: "#",
        },
      ],
    };
  },
  props: {},

  methods: {
    // getImg() {
    //   return require(`../assets/images/${this.cards.url}`);
    // },
  },
};
</script>

<style scoped lang="scss">
@import "@/assets/scss/_generics.scss";
a {
  color: #303030;
}

.card {
  background-color: #f2f8fc;
}

.card-container {
  display: inline-block;
}
</style>
