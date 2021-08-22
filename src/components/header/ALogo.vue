<template>
  <a href="#" class="app-logo">
    <img src="../../assets/logo.png" alt="home" />
  </a>
</template>

<script>
export default {
  name: "ALogo",
};
</script>

<style>
.app-logo {
  position: absolute;
  left: 50%;
  top: 50%;
  transform: translateX(-50%) translateY(-50%);
  z-index: 100;
}

.app-logo > img {
  max-width: 20vh;
}
</style>
