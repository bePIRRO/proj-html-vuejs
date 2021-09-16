<template>
  <div class="container my-5">
    <div class="row">
      <div class="col-3 list">
        <ul>
          <li
            v-for="service in services"
            :key="service"
            :class="index === currentContact ? 'selected' : ''"
            @click="setCurrentService(index)"
          >
            {{ service.listName }}
          </li>
        </ul>
      </div>
      <div class="col-9 content">
        <h2></h2>
        <p></p>
        <ul>
          <li></li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Services",
  props: ["service"],
  data() {
    return {
      currentService: 0,
      services: [
        {
          listName: "What We Do",
          title: "Learning Possibilities",
          text:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Perferendis eaque possimus provident nemo. Animi delectus eos eligendi voluptatem. Velit ullam molestiae vero qui, iusto accusantium. Illo ea quas veritatis aliquam.",
          list: {
            first: "We enrich lives throught learning.",
            second: "Maximizing potential through individual attention.",
            third: "The trusted name for specialized training",
            fourth: "People teach. People learn. This is where they connect.",
          },
          img: "h3-custom-icon-4.png",
        },

        {
          listName: "Degree Programme",
          title: "Learning Possibilities",
          text:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Perferendis eaque possimus provident nemo. Animi delectus eos eligendi voluptatem. Velit ullam molestiae vero qui, iusto accusantium. Illo ea quas veritatis aliquam.",
          list: {
            first: "We enrich lives throught learning.",
            second: "Maximizing potential through individual attention.",
            third: "The trusted name for specialized training",
            fourth: "People teach. People learn. This is where they connect.",
          },
          img: "h3-custom-icon-1.png",
        },

        {
          listName: "Career Achievements",
          title: "Learning Possibilities",
          text:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Perferendis eaque possimus provident nemo. Animi delectus eos eligendi voluptatem. Velit ullam molestiae vero qui, iusto accusantium. Illo ea quas veritatis aliquam.",
          list: {
            first: "We enrich lives throught learning.",
            second: "Maximizing potential through individual attention.",
            third: "The trusted name for specialized training",
            fourth: "People teach. People learn. This is where they connect.",
          },
          img: "h3-custom-icon-3.png",
        },

        {
          listName: "Personal Managment",
          title: "Learning Possibilities",
          text:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Perferendis eaque possimus provident nemo. Animi delectus eos eligendi voluptatem. Velit ullam molestiae vero qui, iusto accusantium. Illo ea quas veritatis aliquam.",
          list: {
            first: "We enrich lives throught learning.",
            second: "Maximizing potential through individual attention.",
            third: "The trusted name for specialized training",
            fourth: "People teach. People learn. This is where they connect.",
          },
          img: "h3-custom-icon-5.png",
        },

        {
          listName: "Steps To Success",
          title: "Learning Possibilities",
          text:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Perferendis eaque possimus provident nemo. Animi delectus eos eligendi voluptatem. Velit ullam molestiae vero qui, iusto accusantium. Illo ea quas veritatis aliquam.",
          list: {
            first: "We enrich lives throught learning.",
            second: "Maximizing potential through individual attention.",
            third: "The trusted name for specialized training",
            fourth: "People teach. People learn. This is where they connect.",
          },
          img: "h3-custom-icon-2.png",
        },

        {
          listName: "Knowledge Transfer",
          title: "Learning Possibilities",
          text:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Perferendis eaque possimus provident nemo. Animi delectus eos eligendi voluptatem. Velit ullam molestiae vero qui, iusto accusantium. Illo ea quas veritatis aliquam.",
          list: {
            first: "We enrich lives throught learning.",
            second: "Maximizing potential through individual attention.",
            third: "The trusted name for specialized training",
            fourth: "People teach. People learn. This is where they connect.",
          },
          img: "h3-custom-icon-6.png",
        },
      ],
    };
  },

  methods: {
    setCurrentService(index) {
      this.currentService = index;
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

  &.selected {
    color: $link-color;
    border-left: 7px solid $link-color;
  }

  &:hover {
    cursor: pointer;
  }
}
</style>
