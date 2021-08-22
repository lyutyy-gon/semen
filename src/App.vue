<template>
  <div>
    <AHeader :isHeaderActive="isHeaderActive" />
    <ABody />
  </div>
</template>

<script>
import AHeader from "./components/header/AHeader";
import ABody from "./components/body/ABody"

export default {
  name: "App",
  data() {
    return {
      isHeaderActive: true,
    };
  },
  components: {
    AHeader,
    ABody
  },
  mounted() {
    document.addEventListener("scroll", () => {
      if (window.pageYOffset > 0) {
        this.isHeaderActive = false;
      } else {
        this.isHeaderActive = true;
      }
    });
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;500;600;700&display=swap");

body {
  font-family: "Playfair Display", serif;
  background: #f1f0ec;
  color: #31312e;
  height: 2000px;
}

* {
  margin: 0px;
  padding: 0px;
}

a {
  text-decoration: none;
  letter-spacing: 0.13em;
}

input,
button {
  outline: none;
  border: none;
}

input {
  padding: 10px;
}

input[type="submit"]:hover {
  cursor: pointer;
}
</style>
