<template>
  <div class="app-right-side">
    <img class="img" src="../../assets/bgPositive.jpg" alt="">
  </div>
</template>

<script>
export default {
  name: "ARightSide",
};
</script>

<style>
.app-right-side {
  position: fixed;
  right: 0px;
  width: 50%;
  overflow: hidden;
  /* background: 0px / cover no-repeat url("../../assets/bgPositive.jpg"); */
}

.app-right-side .img {
  height: 100vh;
}
</style>