<template>
  <div class="container-fluid me-0 button-container">
    <div class="container my-5">
      <div class="row">
        <div class="col-3 list">
          <ul>
            <li
              @click="setCurrentService(index)"
              v-for="(service, index) in services"
              :key="service.index"
              :class="currentService === service.index ? 'selected' : ''"
            >
              {{ service.listName }}
            </li>
          </ul>
        </div>
        <div class="col-9 content">
          <h2>{{ services[currentService].title }}</h2>
          <p>{{ services[currentService].text }}</p>
          <ul class="check-list">
            <li v-for="text in list" :key="text" class="text-start">
              {{ text }}
            </li>
          </ul>
          <figure>
            <img src="getImg(services[currentService].img)" alt="img" />
          </figure>
        </div>
      </div>
    </div>
    <TopButton class="pos-left" />
  </div>
</template>

<script>
import TopButton from "./TopButton.vue";

export default {
  name: "Services",
  props: ["service"],
  components: { TopButton },
  data() {
    return {
      currentService: 0,
      services: [
        {
          listName: "What We Do",
          title: "Learning Possibilities",
          text:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Perferendis eaque possimus provident nemo. Animi delectus eos eligendi voluptatem. Velit ullam molestiae vero qui, iusto accusantium. Illo ea quas veritatis aliquam.",
          img: "h3-custom-icon-4.png",
        },

        {
          listName: "Degree Programme",
          title: "Degree Programme",
          text:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Perferendis eaque possimus provident nemo. Animi delectus eos eligendi voluptatem. Velit ullam molestiae vero qui, iusto accusantium. Illo ea quas veritatis aliquam.",
          img: "h3-custom-icon-1.png",
        },

        {
          listName: "Career Achievements",
          title: "Career Achievements",
          text:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Perferendis eaque possimus provident nemo. Animi delectus eos eligendi voluptatem. Velit ullam molestiae vero qui, iusto accusantium. Illo ea quas veritatis aliquam.",
          img: "h3-custom-icon-3.png",
        },

        {
          listName: "Personal Managment",
          title: "Personal Managment",
          text:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Perferendis eaque possimus provident nemo. Animi delectus eos eligendi voluptatem. Velit ullam molestiae vero qui, iusto accusantium. Illo ea quas veritatis aliquam.",
          img: "h3-custom-icon-5.png",
        },

        {
          listName: "Steps To Success",
          title: "The Way To Success",
          text:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Perferendis eaque possimus provident nemo. Animi delectus eos eligendi voluptatem. Velit ullam molestiae vero qui, iusto accusantium. Illo ea quas veritatis aliquam.",
          img: "h3-custom-icon-2.png",
        },

        {
          listName: "Knowledge Transfer",
          title: "Work around the world",
          text:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Perferendis eaque possimus provident nemo. Animi delectus eos eligendi voluptatem. Velit ullam molestiae vero qui, iusto accusantium. Illo ea quas veritatis aliquam.",
          img: "h3-custom-icon-6.png",
        },
      ],
      list: [
        "We enrich lives throught learning.",
        "Maximizing potential through individual attention.",
        "The trusted name for specialized training",
        "People teach. People learn. This is where they connect.",
      ],
    };
  },

  methods: {
    setCurrentService(index) {
      this.currentService = index;
    },

    getImg() {
      return require(`@/assets/img/${this.services.img}`);
    },
  },
};
</script>

<style scoped lang="scss">
@import "../assets/scss/_generics.scss";

.list {
  li {
    list-style-type: none;
    background-color: #fcfcfc;
    border: 1px solid #e5e5e5;
    color: #847b7b;
    padding: 20px 0;
  }

  li:hover {
    cursor: pointer;
    color: $link-color;
    border-left: 7px solid $link-color;
  }
}

.selected {
  color: $link-color;
  border-left: 7px solid $link-color;
}

.check-list {
  li {
    list-style-type: none;

    &::before {
      font-family: "Font Awesome 5 free";
      content: "\f00c";
      color: $link-color;
      display: inline-block;
      vertical-align: middle;
      width: 10px;
      margin-left: 5px;
    }
  }
}
</style>
