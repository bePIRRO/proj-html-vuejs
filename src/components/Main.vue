<template>
  <!-- print cards -->
  <main class="m-5 me-0">
    <div v-for="card in cards" :key="card" class="card-container mx-4 mb-5">
      <Card :card="card" />
    </div>

    <!-- main article -->
    <section class="text-start mx-5 button-container">
      <div class="mt-5">
        <h1>The Trusted Name</h1>
        <h1>for In-Home Tutoring</h1>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Officia
          tenetur aliquam dolorum atque, necessitatibus reprehenderit illo sint,
          beatae ab assumenda praesentium consectetur nemo vitae. Ipsum porro
          aut unde illum facilis.
        </p>
        <a href="#">LEARN MORE</a>
      </div>
      <img src="../assets/img/h5-img-1.jpg" alt="" />
      <TopButton />
    </section>

    <!-- world datas -->
    <section class="text-start m-5">
      <div class="row me-1 button-container">
        <div class="col-6">
          <img src="../assets/img/h1-img-8.jpg" alt="" />
        </div>
        <div class="col-6">
          <h1 class="mb-3">Empowering Children to Reach Their Potential.</h1>
          <p class="my-4">
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Officiis
            quos quasi et. Error consectetur, facere nisi dolore architecto,
            eveniet nihil vero, suscipit pariatur ipsam animi amet quaerat quas
            eligendi fugit.
          </p>
          <div class="col-6 datas mt-4">
            <h2>168</h2>
            User Stories
          </div>
          <div class="col-6 datas mt-4">
            <h2>347</h2>
            Events
          </div>
        </div>
        <TopButton />
      </div>
    </section>
  </main>
</template>

<script>
import Card from "@/components/Card.vue";
import TopButton from "./TopButton.vue";

export default {
  name: "Main",
  props: ["card"],
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
          text: "DIY&Craft",
          link: "#",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "../assets/scss/_generics.scss";
@import "../assets/scss/_card.scss";
a {
  color: #40c4ff;
  font-weight: 600;
}

p {
  font-size: 1.4em;
}

h1 {
  font-size: 4.5em;
}
</style>
