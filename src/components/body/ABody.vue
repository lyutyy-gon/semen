<template>
  <div>
    <ALeftSide />
    <ARightSide />
    <AContent />
  </div>
</template>

<script>
import ALeftSide from "./ALeftSide";
import ARightSide from "./ARightSide";
import AContent from "./AContent";

export default {
  name: "ABody",
  components: {
    ALeftSide,
    ARightSide,
    AContent,
  },
};
</script>
