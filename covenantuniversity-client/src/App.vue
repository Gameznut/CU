<template>
  <div>
    <nav class="flex justify-between items-center fixed bg-white w-full">
      <div>
        <img alt="Cu logo" src="./assets/Culogo.png" />
      </div>
      <div class="mx-4" v-for="link in links" :key="link.tos">
        <router-link :to="link.tos">{{ link.name }}</router-link>
      </div>
    </nav>
    <div>
      <router-view />
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      links: [
        {
          name: "Home",
          tos: "/",
        },
        {
          name: "About",
          tos: "about",
        },
        {
          name: "Study",
          tos: "about",
        },
        {
          name: "Admissions",
          tos: "about",
        },
        {
          name: "campus life",
          tos: "about",
        },
        {
          name: "imformation",
          tos: "about",
        },
        {
          name: "researching & teaching",
          tos: "about",
        },
        {
          name: "Alumni",
          tos: "about",
        },
      ],
    };
  },
};
</script>
