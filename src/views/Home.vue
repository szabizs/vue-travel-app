<template>
  <div class="home"></div>
</template>

<script>
// @ is an alias to /src
import store from "@/store.js";

export default {
  name: "Home",
  components: {},
  data() {
    return {
      destination: store.destination,
    };
  },
};
</script>
