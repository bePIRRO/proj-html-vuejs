<template>
  <main class="m-5">
    <div v-for="card in cards" :key="card.index">
      <Card />
    </div>

    <div class="text-start">
      <div class="">
        <h1>The Trusted Name for In-Home Tutoring</h1>
      </div>
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Officia tenetur
        aliquam dolorum atque, necessitatibus reprehenderit illo sint, beatae ab
        assumenda praesentium consectetur nemo vitae. Ipsum porro aut unde illum
        facilis.
      </p>
      <a href="#">LEARN MORE</a>
      <figure>
        <img src="../assets/img/h5-img-1.jpg" alt="" />
      </figure>
      <TopButton />
    </div>
  </main>
</template>

<script>
import Card from "@/components/Card.vue";
import TopButton from "./TopButton.vue";

export default {
  name: "Main",
  components: {
    Card,
    TopButton,
  },
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
};
</script>

<style scoped>
@import "../assets/scss/_generics.scss";

a {
  color: #40c4ff;
  font-weight: 600;
}
</style>
