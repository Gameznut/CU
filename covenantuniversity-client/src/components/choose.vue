<template>
  <div class="bg-purple-800 relative text-white">
    <img class="opacity-10 w-full imgs" src="../assets/alumni-bg.jpg" alt="" />
    <div class="mx-80 absolute z-30 top-0 h-full">
      <div>
        <h1 class="text-center text-5xl font-bold py-10">
          Why Choose Covenant ?
        </h1>
        <div class="grid grid-cols-3 gap-8">
          <div v-for="card in cards" :key="card">
            <img class="" :src="card.image" alt="" />
            <h1 class="mt-12 mb-3 text-3xl font-bold">{{ card.title }}</h1>
            <p class="text-lg mb-14">{{ card.text }}</p>
          </div>
        </div>
        <div class="flex justify-center">
            <button class="p-3 my-5 rounded-lg hover:text-white hover:bg-green-700 bg-gray-100 text-purple-800">More About Why Study At Covenant ></button>
        </div>
        
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      cards: [
        {
          title: "Comprehensive Education",
          text: "Degree programmes at Covenant University are all-encompassing.  The University has developed custom-built courses to specially package the student and deliver him to his world upon graduation as an agent of change. He takes charge of his environment and breaks the barriers of limitation confronting our nation and continent at large.",
          image: require("../assets/education.jpg"),
        },
        {
          title: "Resources",
          text: "The library is the heart and lifeline of any citadel of learning. The library complex is an edifice with three floors, reputed to be one of the largest in Africa. The total floor area of the complex is 11,300m",
          image: require("../assets/learning.jpg"),
        },
        {
          title: "Financial Aid",
          text: "Covenant University offers international scholarships, fellowships, or grants to both local and international students. Apart from university-based scholarships, many other organizations, including foundations, trusts, and corporate bodies, give scholarships to international students.",
          image: require("../assets/financial.jpg"),
        },
        {
          title: "Active Alumni Network",
          text: "The University has Alumni network with more than 10,000 engaged members in more than 50 countries, exclusive alumni platform and job opportunities, more than 15% Alumni are Entrepreneurs (Job Creators) and Graduates excel as Ivy League Postgraduate students",
          image: require("../assets/alumini.jpg"),
        },
        {
          title: "Campus",
          text: "Covenant's campus is an ultra-modern new generation campus. Her luscious lawns, beautifully planned gardens and architectural masterpiece buildings provide a unique, stimulating and empowering context for inspiring research and creative activities.",
          image: require("../assets/covenant.jpg"),
        },
        {
          title: "Global Rankings",
          text: "Covenant University has had a rapid rise in nearly two decades of its existence. The webometric ranking named Covenant University the best Private University in Nigeria in its 2021 ranking and the second best university overall.",
          image: require("../assets/award.jpg"),
        },
      ],
    };
  },
};
</script>
<style>
.imgs{
    width: 100%;
    height: 1490px;
}
    
</style>