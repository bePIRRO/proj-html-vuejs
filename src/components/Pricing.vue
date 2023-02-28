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
            <li v-for="text in type" :key="text" class="list-table">
              {{ text }}
            </li>
          </ul>
        </div>

        <!-- standard -->
        <div class="col-2 list" id="standard">
          <ul>
            <li class="list-table">
              <img src="../assets/img/h5-custom-icon-7.png" alt="" />
              <h3>Standard</h3>
              <h4>$12</h4>
            </li>
            <li v-for="item in standard" :key="item" class="list-table">
              {{ item }}
              <i class="fas"></i>
              <!-- :class="(item = '1' ? 'fa-check' : 'fa-times')" -->
            </li>
            <li class="bg-blue">
              <div class="btn btn-white my-5 rounded-0">
                <a href="#">GET IT NOW</a>
              </div>
            </li>
          </ul>
        </div>

        <!-- professional -->
        <div class="col-2 list" id="pro">
          <ul>
            <li class="list-table">
              <img src="../assets/img/h5-custom-icon-8.png" alt="" />
              <h3>Professional</h3>
              <h4>$59</h4>
            </li>
            <li v-for="item in pro" :key="item" class="list-table">
              {{ item }}
            </li>
            <li class="bg-blue">
              <div class="btn btn-blue my-5 rounded-0">
                <a href="#">GET IT NOW</a>
              </div>
            </li>
          </ul>
        </div>

        <!-- advanced -->
        <div class="col-2 list" id="pro">
          <ul>
            <li class="list-table">
              <img src="../assets/img/h5-custom-icon-9.png" alt="" />
              <h3>Advanced</h3>
              <h4>$88</h4>
            </li>
            <li v-for="item in pro" :key="item" class="list-table">
              {{ item }}
            </li>
            <li class="bg-blue">
              <div class="btn btn-white my-5 rounded-0">
                <a href="#">GET IT NOW</a>
              </div>
            </li>
          </ul>
        </div>
      </div>
    </section>
    <hr />
  </div>
</template>

<script>

export default {
  name: "Pricing",
  data() {
    return {
      type: [
        "Save up to 40% by paying weekly",
        "Number of Courses",
        "Time",
        "Web Designing",
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

  computed: {},
};
</script>

<style scoped lang="scss">
@import "@/assets/scss/_generics.scss";

section {
  padding-bottom: 150px;
}

.list {
  margin: 0;
  padding: 0;

  ul {
    padding: 0;
  }

  .list-table {
    list-style-type: none;
    background-color: #fcfcfc;
    border: 1px solid #e5e5e5;
    color: #847b7b;
    padding: 20px 0;
  }
}

#list li:first-child {
  height: 201px;
  font-size: 1.9em;
  text-align: start;
  padding-left: 15px;
}

.bg-blue {
  background-color: #f7fdff;
  list-style-type: none;
  border: 1px solid #e5e5e5;
}

.btn {
  border: 1px solid #e5e5e5;
}
</style>
