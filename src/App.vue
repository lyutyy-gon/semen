<template>
  <div>
    <AHeader />
  </div>
</template>

<script>
import AHeader from "./components/header/AHeader";

export default {
  name: "App",
  components: {
    AHeader,
  },
};
</script>

<style>
* {
  margin: 0px;
  padding: 0px;
}

a {
  text-decoration: none;
}

input, button {
  outline: none;
  border: none;
}

input {
  padding: 5px;
}

input[type=submit]:hover {
  cursor: pointer;
}
</style>
