<template>
  <div class="app-header">
    <div class="app-header__wrapper">
      <AMenu />
      <ALogo />
      <ACallbackForm />
    </div>
  </div>
</template>

<script>
import AMenu from "./AMenu";
import ALogo from "./ALogo";
import ACallbackForm from "./ACallbackForm";

export default {
  name: "AHeader",
  components: {
    AMenu,
    ALogo,
    ACallbackForm,
  },
};
</script>

<style>
.app-header {
  position: fixed;
  min-width: 100%;
  background: lime;
}

.app-header__wrapper {
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 90%;
  margin: 0px auto;
  padding: 20px 0px;
}
</style>
