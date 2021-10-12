<template>
  <div class="relative">
    <img
      class="opacity-10 w-full img"
      src="../assets/apply-banner2.jpg"
      alt=""
    />
    <div class="mx-80 mt-6 top-0 absolute">
      <div class="">
        <div class="border-purple-800 border-l-8 p-7 space-y-5 my-4">
          <h3 class="text-3xl font-serif text-purple-900">
            Apply to more than 36 areas of study across
          </h3>
          <h1 class="text-5xl text-purple-900 font-serif font-black">
            23 Departments & 4 Colleges
          </h1>
        </div>
        <a
          class="hover:text-green-600 text-purple-900 font-light my-4"
          v-for="(link, index) in linkTo"
          :key="link"
          :href="index"
        >
          {{ link }}
        </a>
        <div class="flex justify-between gap-6 my-4 mt-16">
          <div
            v-for="card in cards"
            :key="card"
            class="flex flex-col justify-between w-3/4 bg-gray-800"
          >
            <img
              :src="card.image"
              class="relative h-60 opacity-70"
              alt="card.title"
            />
            <p class="absolute bottom-9 ml-10 text-3xl text-white font-bold">
              {{ card.title }}
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      linkTo: {
        engineering: "Engineering | ",
        "science-and-technology": "Science and Technology | ",
        "management-and-social-sciences": "Management and Social Sciences | ",
        "leadership-and-development-studies":
          "Leadership-and Development Studies | ",
        "postgraduate-studies": "Postgraduate Studies",
      },
      cards: [
        {
          title: "Postgraduate",
          image: require("../assets/post-graduate.jpg"),
        },
        {
          title: "Undergraduate",
          image: require("../assets/undersgraduate.jpg"),
        },
        {
          title: "International Student",
          image: require("../assets/international.png"),
        },
      ],
    };
  },
};
</script>
<style>
.img {
  height: 600px;
}
</style>
