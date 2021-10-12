<template>
  <div>
    <div class="flex mx-6 gap-x-7 justify-between">
      <img class="w-2/4" src="../assets/welcome.jpg" alt="welcome" />
      <div class="space-y-8 mt-28 w-9/12">
        <h1 class="text-3xl font-bold text-purple-900">ABOUT US</h1>
        <p class="text-xl text-purple-900">
          Covenant University is a growing, dynamic vision-driven University,
          founded on a Christian mission ethos and committed to pioneering
          excellence at the cutting edge of learning. We run with a compelling
          vision of raising a new generation of leaders for the African
          continent. We are doing this on a holistic, human development and
          integrated learning curriculum to raise total Men and Women who will
          develop their world.
        </p>
        <p class="text-xl text-purple-900">
          Our Core-Values of Spirituality, Possibility Mentality, Capacity
          Building, Integrity, Responsibility, Diligence, and Sacrifice are what
          defines our commitment to excellence.
        </p>
        <button
          class="
            bg-purple-900
            text-white
            hover:bg-green-600
            px-5
            rounded-xl
            py-5
            font-bold
          "
        >
          Read more >
        </button>
      </div>
      <div class="mt-8">
        <div
          v-for="(link, to) in links"
          :key="link"
          class="my-1 flex text-center flex-col"
        >
          <a
            class="bg-purple-300 py-2 px-20 rounded-md hover:bg-green-400"
            :href="to"
            >{{ link }}</a
          >
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      links: {
        apply: "Apply",
        visit: "VisitCampus",
        student: "Student",
        library: "Library",
        scholarship: "Scholarship",
        event: "Event",
        faq: "FAQ",
      },
    };
  },
};
</script>
<style>
:hover.fade-enter-active,
.fade-leave-active {
  background-color: aquamarine;
  transition: opacity 0.3s ease;
}

:hover.fade-enter-from,
.fade-leave-to {
  background-color: aquamarine;
  opacity: 1;
}
</style>
