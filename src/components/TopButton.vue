<template>
  <a href="#header">
    <div class="text-center">
      <i class="fas fa-angle-up fa-2x m-0 p-0"></i>
      <h6 class="m-0 p-0">TOP</h6>
    </div>
  </a>
</template>

<script>
export default {
  name: "TopButton",
};
</script>

<style scoped lang="scss">
@import "../assets/scss/_generics.scss";
div {
  display: inline-block;
  background-color: $link-color;
  color: $white;
  width: 54px;
  position: absolute;
  left: 99%;
  top: 90%;
}
</style>
