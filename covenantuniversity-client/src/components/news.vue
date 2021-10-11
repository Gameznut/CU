<template>
  <div class="mx-80 mt-6">
    <div class="bg-black w-full flex items-center">
      <div
        class="h-10 w-4/12 flex bg-green-600 rounded-tr-full rounded-br-full"
      >
        <p class="flex mx-auto items-center">Latest News</p>
      </div>
      <p class="text-white mx-10">
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
    <div  class="flex justify-between gap-4">
      <div v-for="newz in news" :key="newz">
        <img :src="newz.images" :alt="newz.title" />
        <h1 class="text-center">{{ newz.title }}</h1>
        <p class="text-center">{{ newz.text }}</p>
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
          images: "../assets/rank.jpg",
        },
        {
          title: "NOTICE",
          text: "Important Notifications and announcements to all our students",
          btnTitle: "SEE NOTICE BOARD >",
          images: "../assets/notice.png",
        },
        {
          title: "ADMISSION NOW",
          text: "For information that will assist our propective students to study at Covenant",
          btnTitle: "APPLY NOW >",
          images: "../assets/admission.png",
        },
      ],
    };
  },
};
</script>
