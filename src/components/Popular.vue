<template>
  <section class="container">
    <div class="row">
      <div class="col-12">
        <h2>Popular Online Courses</h2>
        <p>
          Lorem ipsum, dolor sit amet consectetur adipisicing elit. Nihil
          officiis dolorum est. Exercitationem, aliquid autem a assumenda sed et
          animi tenetur dolor excepturi impedit possimus illo unde quia
          perferendis deserunt!
        </p>
      </div>
    </div>
    <div class="row d-flex">
      <div class="col-4 card text-start p-0">
        <img src="../assets/img/course-5-f-img.jpg" alt="" class="img-fluid" />
        <div class="row">
          <div class="col-7 ms-2">
            <h5>Android Developer</h5>
            <p>David Sanders</p>
          </div>
          <div class="col-4">
            <span class="tag free">
              FREE
            </span>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Popular",
};
</script>

<style scoped lang="scss">
@import "../assets/scss/_generics.scss";
.container {
  background-image: url("../assets/img/background-pattern.jpg");
}

.card {
  border: 1px solid #847b7b;

  p {
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
</style>
