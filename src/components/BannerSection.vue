<template>
  <div class="banner">
    <div class="banner__img">
      <img src="../assets/img/banner.jpg" alt="">
    </div>
    <div class="banner__bg"> </div>
  </div>
</template>

<script setup>

</script>

<style lang="scss" scoped>
.banner {
  margin-bottom: 50px;
  margin-top: 20px;
  height: 400px;
  position: relative;

  // overflow: hidden;
  &__img {
    width: 350px;
    height: 400px;
    position: relative;
    box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;
    z-index: 2;

    >img {
      width: 100%;
      height: 100%;
    }
  }

  &__bg {
    width: 350px;
    height: 400px;
    background-color: #8b7e6d;
    position: absolute;
    top: 0;
    z-index: 1;
    transform: rotate(8deg);
    box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;
  }
}
</style>
