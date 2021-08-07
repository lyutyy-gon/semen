<template>
  <form class="app-form">
    <input type="text" name="mail" placeholder="Ваша почта:" />
    <input type="text" name="question" placeholder="Ваш вопрос:" />
    <input type="submit" value="Send" />
  </form>
</template>

<script>
export default {
  name: "ACallbackForm",
  components: {},
};
</script>

<style>
.app-form {
  display: flex;
  flex-direction: column;
}

.app-form > input:not([type=submit]) {
  margin-bottom: 5px;
}
</style>
