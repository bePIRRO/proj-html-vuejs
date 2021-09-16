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
        <!-- list -->
        <div class="col-2 list" id="list">
          <ul>
            <li v-for="text in type" :key="text">{{ text }}</li>
          </ul>
        </div>

        <!-- standard -->
        <div class="col-2 list" id="standard">
          <ul>
            <li>
              <img src="../assets/img/h5-custom-icon-7.png" alt="" />
              <h3>Standard</h3>
              <h4>$12</h4>
            </li>
            <li v-for="item in standard" :key="item">
              {{ item }}
            </li>
          </ul>
        </div>

        <!-- professional -->
        <div class="col-2 list" id="pro">
          <ul>
            <li>
              <img src="../assets/img/h5-custom-icon-8.png" alt="" />
              <h3>Professional</h3>
              <h4>$59</h4>
            </li>
            <li v-for="item in pro" :key="item">
              {{ item }}
            </li>
          </ul>
        </div>

        <!-- advanced -->
        <div class="col-2 list" id="pro">
          <ul>
            <li>
              <img src="../assets/img/h5-custom-icon-9.png" alt="" />
              <h3>Advanced</h3>
              <h4>$88</h4>
            </li>
            <li v-for="item in pro" :key="item">
              {{ item }}
            </li>
          </ul>
        </div>
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
      type: [
        "Save up to 40% by paying weekly",
        "Number of Courses",
        "Time",
        "Human-Centered Design",
        "Basic Marketing",
        "Python for Everybody",
        "Android Developer",
        "Business English",
      ],

      standard: {
        num: 2,
        time: "15 Days",
        web: true,
        human: false,
        marketing: false,
        phyton: false,
        android: false,
        business: false,
      },

      pro: {
        num: 2,
        time: "30 Days",
        web: true,
        human: true,
        marketing: true,
        phyton: true,
        android: false,
        business: false,
      },

      advanced: {
        num: 2,
        time: "30 Days",
        web: true,
        human: true,
        marketing: true,
        phyton: true,
        android: false,
        business: false,
      },
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

#list li:first-child {
  height: 200px;
  font-size: 1.9em;
  text-align: start;
  padding-left: 15px;
}
</style>
