<template>
  <div class="app-form">
    <form class="app-form__wrapper">
      <input type="text" name="mail" placeholder="Ваша почта:" />
      <input type="text" name="question" placeholder="Ваш вопрос:" />
      <input type="submit" value="Отправить" />
    </form>
  </div>
</template>

<script>
export default {
  name: "ACallbackForm",
  components: {},
};
</script>

<style>
.app-form {
  position: relative;
  flex-basis: 50%;
}

.app-form__wrapper {
  display: flex;
  flex-direction: column;
  max-width: 50%;
  margin: 0px auto;
  position: absolute;
  min-width: 50%;
  top: 50%;
  left: 50%;
  transform: translateX(-50%) translateY(-50%);
}

.app-form__wrapper > input {
  border-radius: 10px;
  background: #f1f0ec;
  color: #31312e;
}

.app-form__wrapper > input:not([type="submit"]) {
  margin-bottom: 5px;
}

.app-form__wrapper > input[type="submit"] {
  background: #f8da7e;
}
</style>
