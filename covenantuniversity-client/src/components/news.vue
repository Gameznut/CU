<template>
  <div class="mx-80 mt-6">
    <div class="bg-black w-full flex items-center">
      <div
        class="h-10 w-4/12 flex bg-green-600 rounded-tr-full rounded-br-full"
      >
        <p class="flex mx-auto items-center text-white text-base">
          Latest News
        </p>
      </div>
      <p class="text-white mx-10 hover:text-green-700 font-semibold text-base">
        Professor Adebayo Seeks Renewed Commitment to Food Security in Nigeria
      </p>
      <div class="flex ml-36">
        <!-- left -->
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="h-10 w-10"
          fill="purple"
          viewBox="0 0 24 24"
          stroke="white"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M11 19l-7-7 7-7m8 14l-7-7 7-7"
          />
        </svg>
        <!-- right -->
        <svg
          xmlns="http://www.w3.org/2000/svg"
          className="h-10 w-10"
          fill="purple"
          viewBox="0 0 24 24"
          stroke="white"
        >
          <path
            strokeLinecap="round"
            strokeLinejoin="round"
            stroke-width="2"
            d="M13 5l7 7-7 7M5 5l7 7-7 7"
          />
        </svg>
      </div>
    </div>
    <!-- news card -->
    <div class="flex justify-between gap-6 mt-3 my-4">
      <div
        v-for="newz in news"
        :key="newz"
        class="flex flex-col justify-between w-3/4 bg-gray-200"
      >
        <img class="w-full h-max" :src="newz.images" :alt="newz.title" />
        <h1 class="text-center text-2xl font-extrabold my-10">
          {{ newz.title }}
        </h1>
        <p class="text-center mx-auto px-20 text-md">{{ newz.text }}</p>
        <button
          class="
            px-3
            py-2
            mt-20
            mx-auto
            bg-purple-700
            hover:bg-pink-500
            rounded-md
          "
        >
          {{ newz.btnTitle }}
        </button>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      news: [
        {
          title: "GLOBAL RANKING",
          text: "Covenant, the only Nigerian University featured Rises 50 Places to 101-150 in THE Young University Rankings",
          btnTitle: "LEARN MORE >",
          images: require("../assets/1.png"),
        },
        {
          title: "NOTICE BOARD",
          text: "Important Notifications and announcements to all our students",
          btnTitle: "SEE NOTICE BOARD >",
          images: require("../assets/2.png"),
        },
        {
          title: "ADMISSION NOW",
          text: "For information that will assist our propective students to study at Covenant",
          btnTitle: "APPLY NOW >",
          images: require("../assets/3.png"),
        },
      ],
    };
  },
};
</script>
