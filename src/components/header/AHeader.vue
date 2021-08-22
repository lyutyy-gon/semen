<template>
  <div class="app-header">
    <ALogo />
    <div
      class="app-header__wrapper"
      :class="{
        'app-header__active': isHeaderActive,
        'app-header__passive': !isHeaderActive,
      }"
    >
      <AMenu />
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
  props: ["isHeaderActive"],
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
  background: rgba(0, 0, 0, 0.7);
  z-index: 100;
}

.app-header__wrapper {
  display: flex;
}

.app-header__active {
  min-height: 90vh;
  transition: min-height 0.5s ease-out;
}

.app-header__passive {
  min-height: 25vh;
  transition: min-height 0.5s ease-out;
}
</style>
