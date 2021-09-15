<template>
  <header class="pb-5" id="header">
    <MainNav />
    <div class="my-5 py-5 container">
      <h1 class="display-1 my-5">Contemporary Ideas</h1>
      <p class="h5">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Magnam numquam
        asperiores veritatis corrupti eius cupiditate laboriosam officiis
        voluptas fugit a labore, praesentium totam quam repellendus, quae ea qui
        nesciunt eligendi.
      </p>

      <div class="btn btn-blue my-5 border-0 rounded-0">
        <a href="#">REGISTER NOW</a>
      </div>
    </div>
    <Slider />
  </header>
</template>

<script>
import MainNav from "./MainNav.vue";
import Slider from "./Slider.vue";

export default {
  name: "Header",
  components: {
    MainNav,
    Slider,
  },
  props: {},
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/_generics.scss";

header {
  background-image: url("../assets/img/h5-slide-3-background.jpg");
  background-repeat: no-repeat;
  background-size: cover;
  height: auto;
  color: #fff;
}
</style>
