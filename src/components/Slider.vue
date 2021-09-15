<template>
  <div id="slider">
    <ul class="p-0">
      <li v-for="index in 3" :key="index">
        <i class="fa-dot-circle" :class="isActive ? 'far' : 'fas'"></i>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "Slider",
  props: {},
};
</script>

<style scoped lang="scss">
li {
  list-style-type: none;
  display: inline-block;

  i {
    margin: 0 10px;
  }
}
</style>
