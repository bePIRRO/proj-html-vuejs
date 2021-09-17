<template>
  <section class="container-fluid button-container text-start">
    <div class="container">
      <div class="row">
        <!-- info col -->
        <div class="col-3">
          <img
            src="../assets/img/logo-light.png"
            alt="iAcademy-logo"
            class="img-fluid logo"
          />
          <p>
            Providing Life Changing Experiences Through Education. Class That
            Fit Your Busy Life. Closer to Home
          </p>
          <div class="tel my-4">
            <i class="fas fa-phone"></i>
            1-677-124-44227
          </div>
          <div class="time pb-5">
            <i class="far fa-clock"></i>
            Mon - Sat 8.00 - 18.00
          </div>
        </div>

        <!-- popular courses col -->
        <div class="col-3">
          <h3>Popular Courses</h3>
          <div class="course">
            <a href="#" class="h5">Business Englis</a>
            <h6>Preston Marshall</h6>
          </div>

          <div class="course my-4">
            <a href="#" class="h5">Socical computing</a>
            <h6>David Sanders</h6>
          </div>

          <div class="course">
            <a href="#" class="h5">Learn Spanish</a>
            <h6>Jennie King</h6>
          </div>
        </div>

        <!-- support col -->
        <div class="col-3">
          <h3>Support</h3>
          <ul class="p-0">
            <li>
              <a href="#">User dashbord</a>
            </li>
            <li>
              <a href="#">Contac Us</a>
            </li>
            <li>
              <a href="#">FAQ</a>
            </li>
            <li>
              <a href="#">Course Offer</a>
            </li>
            <li>
              <a href="#">Events</a>
            </li>
          </ul>
        </div>

        <!-- map col -->
        <div class="col-3">
          <h3>Flexible Learning</h3>
          <img
            src="../assets/img/footer-img-1.png"
            alt="world"
            class="img-fluid"
          />
        </div>
      </div>
      <hr />

      <!-- copyrights -->
      <div class="row py-5">
        <div class="col-6">
          <p>Copyrights 2017 &#169;Mikado Themes</p>
        </div>
        <div class="col-6 text-end">
          <ul class="p-0">
            <li>
              <a href="#">
                <i class="fas fa-phone"></i>
                +44 300 303 0266
              </a>
            </li>
            <li>FOLLOW US</li>
            <li>
              <a href="#"><i class="fab fa-twitter"></i></a>
            </li>
            <li>
              <a href="#"><i class="fab fa-instagram"></i></a>
            </li>
            <li>
              <a href="#"><i class="fab fa-facebook-f"></i></a>
            </li>
          </ul>
        </div>
      </div>
    </div>
    <TopButton class="pos-left" />
  </section>
</template>

<script>
import TopButton from "./TopButton.vue";

export default {
  name: "Main",
  props: {},
  components: { TopButton },
  data() {},
};
</script>

<style scoped lang="scss">
@import "../assets/scss/_generics.scss";

section {
  background-color: #222;
  color: $l-grey;
  padding-top: 150px;

  h3 {
    color: $white;
    margin-bottom: 50px;
  }

  a {
    color: $l-grey;
    &:hover {
      color: $white;
    }
  }
}

.logo {
  max-width: 190px;
  margin-bottom: 50px;
}

.tel {
  color: $white;
}

.time {
  color: $white;
}

li {
  list-style-type: none;
  margin: 10px 0;
}

p {
  font-size: 1.2em;
}

hr {
  border-color: $l-grey;
}

.col-6 {
  li {
    display: inline-block;
    margin: 0 20px;
  }
}
</style>
