<template>
  <div class="container-fluid">
    <div class="container">
      <div class="col-12">
        <img
          src="../assets/img/testimonials-standard-2.png"
          alt="Testimonial"
        />
      </div>
      <div class="col-12">
        <p>
          Lorem ipsum, dolor sit amet consectetur adipisicing elit. Rem dicta
          facilis iusto odit blanditiis quis, ab deleniti sunt, voluptatum sint,
          esse praesentium a debitis reiciendis veritatis perspiciatis magnam
          qui repellendus?
        </p>
        <h3 class="mt-5">Joan Collins</h3>
        <h5>STUDENT</h5>
      </div>
      <div class="col-12">
        <Slider />
      </div>
    </div>
  </div>
</template>

<script>
import Slider from "./Slider.vue";
export default {
  name: "Reviews",
  components: {
    Slider,
  },
};
</script>

<style scoped lang="scss">
@import "../assets/scss/_generics.scss";

.container-fluid {
  background-image: url("../assets/img/h5-parallax-img-1.png");
  background-repeat: no-repeat;
  background-size: cover;
  color: $white;

  p {
    color: $white;
  }
}

.container-fluid {
  padding: 130px 0;
}

.col-12:nth-child(2) {
  margin: 45px 0;
}

h3 {
}
</style>
