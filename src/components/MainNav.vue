<template>
  <ul class="main-nav d-flex justify-content-around align-items-center py-5">
    <li>
      <a href="#"
        ><img src="@/assets/img/logo-light.png" alt="iAcademy" class="logo"
      /></a>
    </li>
    <li v-for="item in menu" :key="item" class="nav-links">
      <a :href="item.link">{{ item.text }} </a>
    </li>
    <li><i class="fas fa-search"></i></li>
    <li><i class="fas fa-shopping-bag"></i></li>
    <li><i class="fas fa-bars"></i></li>
  </ul>
</template>

<script>
export default {
  name: "MainNav",
  data() {
    return {
      menu: [
        {
          link: "#",
          text: "HOME",
        },
        {
          link: "#",
          text: "COURSES",
        },
        {
          link: "#",
          text: "INSTRUCTORS",
        },
        {
          link: "#",
          text: "EVENTS",
        },
        {
          link: "#",
          text: "PAGES",
        },
        {
          link: "#",
          text: "ELEMENTS",
        },
      ],
    };
  },
  props: {},
};
</script>

<style scoped>
ul {
  color: #fff;
}

ul a {
  color: #fff;
  text-decoration: none;
}

li {
  list-style-type: none;
  display: inline-block;
}

.logo {
  max-width: 200px;
}
</style>
