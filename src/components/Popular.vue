<template>
  <div class="button-container">
    <section class="container">
      <div class="row">
        <div class="col-12">
          <h2>Popular Online Courses</h2>
          <p>
            Lorem ipsum, dolor sit amet consectetur adipisicing elit. Nihil
            officiis dolorum est. Exercitationem, aliquid autem a assumenda sed
            et animi tenetur dolor excepturi impedit possimus illo unde quia
            perferendis deserunt!
          </p>
        </div>
      </div>

      <!-- card -->
      <div class="row justify-content-center">
        <div class="col-3 card text-start p-0 mx-4">
          <img
            src="../assets/img/course-5-f-img.jpg"
            alt=""
            class="img-fluid"
          />
          <div class="row">
            <div class="col-7 ms-2">
              <h5 class="mt-3">Android Developer</h5>
              <p>David Sanders</p>
            </div>
            <div class="col-4">
              <span class="tag free">
                FREE
              </span>
            </div>
          </div>
          <div class="col-12 p-3">
            <p class="m-0">
              Lorem ipsum dolor, sit amet consectetur adipisicing elit.
              Repudiandae id esse consequatur ab earum porro quasi eligendi.
            </p>
            <p>
              <span>
                <i class="fas fa-user"></i> 1
                <i class="fas fa-tag ms-3"></i> PROGRAMMING
              </span>
            </p>
          </div>
        </div>

        <!-- card -->
        <div class="col-3 card text-start p-0 mx-4">
          <img
            src="../assets/img/course-6-f-img.jpg"
            alt=""
            class="img-fluid"
          />
          <div class="row">
            <div class="col-7 ms-2">
              <h5 class="mt-3">Web Designing</h5>
              <p>David Sanders</p>
            </div>
            <div class="col-4">
              <span class="tag free">
                FREE
              </span>
            </div>
          </div>
          <div class="col-12 p-3">
            <p class="m-0">
              Lorem ipsum dolor, sit amet consectetur adipisicing elit.
              Repudiandae id esse consequatur ab earum porro quasi eligendi.
            </p>
            <p>
              <span>
                <i class="fas fa-user"></i> 1
                <i class="fas fa-tag ms-3"></i> PROGRAMMING
              </span>
            </p>
          </div>
        </div>

        <!-- card -->
        <div class="col-3 card text-start p-0 mx-4">
          <img
            src="../assets/img/course-12-f-img.jpg"
            alt=""
            class="img-fluid"
          />
          <div class="row">
            <div class="col-7 ms-2">
              <h5 class="mt-3">Financial Modeling</h5>
              <p>David Sanders</p>
            </div>
            <div class="col-4">
              <span class="tag free">
                FREE
              </span>
            </div>
          </div>
          <div class="col-12 p-3">
            <p class="m-0">
              Lorem ipsum dolor, sit amet consectetur adipisicing elit.
              Repudiandae id esse consequatur ab earum porro quasi eligendi.
            </p>
            <p>
              <span>
                <i class="fas fa-user"></i> 1
                <i class="fas fa-tag ms-3"></i> PROGRAMMING
              </span>
            </p>
          </div>
        </div>
      </div>
      <TopButton class="pos-left" />
      <Slider class="mt-5" />
    </section>
  </div>
</template>

<script>
import TopButton from "./TopButton.vue";
import Slider from "./Slider.vue";

export default {
  name: "Popular",
  components: {
    TopButton,
    Slider,
  },
};
</script>

<style scoped lang="scss">
@import "../assets/scss/_generics.scss";
.container {
  background-image: url("../assets/img/background-pattern.jpg");
}

.card {
  border: 1px solid #f2f2f2;

  .col-7 p {
    font-size: 14px;
  }
}

.tag {
  border-radius: 30px;
  padding: 5px 10px;
  position: relative;
  top: 30%;
  left: 45%;
}

.free {
  background-color: #ffd740;
  color: $white;
}

span {
  color: #b9b9b9;
}
</style>
