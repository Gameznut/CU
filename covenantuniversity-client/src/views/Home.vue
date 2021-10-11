<template>
  <div>
    <Videodiv />
    <Newsdiv />
  </div>
</template>

<script>
// @ is an alias to /src
import Videodiv from "@/components/video.vue"
import Newsdiv from "@/components/news.vue";

export default {
  name: "Home",
  components: {
    Videodiv,
    Newsdiv,
  },
};
</script>
