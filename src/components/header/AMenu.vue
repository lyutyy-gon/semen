<template>
  <div class="app-menu">
    <div class="app-menu__wrapper">
      <a href="#"> О проекте </a>
      <a href="#"> Вопрос / Ответ </a>
      <a href="#"> Олимпиада </a>
    </div>
  </div>
</template>

<script>
export default {
  name: "AMenu",
};
</script>

<style>
.app-menu {
  position: relative;
  flex-basis: 50%;
}

.app-menu__wrapper {
  display: flex;
  justify-content: center;
  position: absolute;
  min-width: 100%;
  top: 50%;
  left: 50%;
  transform: translateX(-50%) translateY(-50%);
}

.app-menu a {
  color: #f1f0ec;
}

.app-menu a:not(:last-of-type) {
  border-right: 1px solid #f1f0ec;
  padding-right: 10px;
  margin-right: 10px;
}

.app-menu a:last-of-type {
  color: #f8da7e;
}

.app-menu a:hover {
  color: #f1f0ecb0;
}

.app-menu a:last-of-type:hover {
  color: #f8da7ebb;
}
</style>
