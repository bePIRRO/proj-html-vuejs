<template>
  <div class="button-container py-5">
    <section class="container-fluid">
      <div class="row justify-content-center">
        <div class="col-9">
          <h2 class="display-4 mt-5 mb-4">Pricing Plans</h2>
          <p class="my-5">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Suscipit ea
            adipisci labore.
          </p>
        </div>
      </div>
      <div class="row mx-5 justify-content-center">
        <div class="col-2 list">
          <ul>
            <li v-for="text in type" :key="text">{{ text }}</li>
          </ul>
        </div>
        <div class="col-2 list">
          <ul>
            <li></li>
          </ul>
        </div>
        <div class="col-2"></div>
        <div class="col-2"></div>
      </div>
    </section>
    <TopButton />
  </div>
</template>

<script>
import TopButton from "./TopButton.vue";

export default {
  name: "Pricing",
  components: { TopButton },
  data() {
    return {
      type: ["Save up to 40% by paying weekly", "Number of Courses"],
    };
  },
};
</script>

<style scoped lang="scss">
@import "../assets/scss/_generics.scss";

.list {
  margin: 0;
  padding: 0;

  ul {
    padding: 0;
  }

  li {
    list-style-type: none;
    background-color: #fcfcfc;
    border: 1px solid #e5e5e5;
    color: #847b7b;
    padding: 20px 0;
  }
}
</style>
