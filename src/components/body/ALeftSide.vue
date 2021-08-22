<template>
  <div class="app-left-side">
    <img class="img" src="../../assets/bgNegative.jpg" alt="">
  </div>
</template>

<script>
export default {
  name: "ALeftSide",
};
</script>

<style>
.app-left-side {
  position: fixed;
  min-width: 100vw;
  min-height: 100vh;
  overflow: hidden;
  /* background: 0px / cover no-repeat url('../../assets/bgNegative.jpg'); */
}

.app-left-side .img {
  height: 100vh;
}
</style>