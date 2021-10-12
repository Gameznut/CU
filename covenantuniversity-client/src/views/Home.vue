<template>
  <div>
    <Videodiv />
    <Newsdiv />
    <Departmentdiv />
    <Aboutdiv />
    <Choosediv />
  </div>
</template>

<script>
// @ is an alias to /src
import Videodiv from "@/components/video.vue";
import Newsdiv from "@/components/news.vue";
import Departmentdiv from "@/components/department.vue";
import Aboutdiv from "@/components/about.vue";
import Choosediv from "@/components/choose.vue";

export default {
  name: "Home",
  components: {
    Videodiv,
    Newsdiv,
    Departmentdiv,
    Aboutdiv,
    Choosediv,
  },
};
</script>
