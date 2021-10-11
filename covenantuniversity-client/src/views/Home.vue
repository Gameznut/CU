<template>
  <div class="home">
    <img alt="Cu logo" src="../assets/Culogo.png" />
    <Navbar msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script>
// @ is an alias to /src
import Navbar from "@/components/navbar.vue";

export default {
  name: "Home",
  components: {
    Navbar,
  },
};
</script>
