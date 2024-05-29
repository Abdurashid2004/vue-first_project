<template>
  <div>
    <h2 class="text-center text-3xl font-bold">Our Blog Posts</h2>
    <p class="text-center py-8 text-lg text-slate-400">
      We are an online plant shop offering a wide range of cheap and trendy
      plants.
    </p>
  </div>
  <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-4 gap-8 mb-11">
    <div v-for="(blog, index) in blogs" :key="index" class="flex flex-col">
      <div class="mb-4">
        <img :src="blog.image" alt="Blog Image" class="w-full h-auto" />
      </div>
      <div class="">
        <span class="font-semibold block text-green-500">{{ blog.title }}</span>
        <h3 class="text-2lg font-bold mb-2 w-[189px]">{{ blog.name }}</h3>
        <p class="mb-4 text-slate-400">{{ blog.text }}</p>
        <div class="flex items-center">
          <a :href="blog.link" class="hover:text-green-500">{{ blog.link }}</a>
          <span v-if="blog.icon" v-html="blog.icon" class="ml-2"></span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      blogs: [
        {
          image: "../src/assets/blog1.jpg",
          title: "September 12 | Read in 6 minutes",
          name: "Cactus & Succulent Care Tips",
          text: "Cacti and succulents are easy care plants for any home or patio.",
          link: "Read More",
          icon: `<svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" viewBox="0 0 24 24"><path fill="none" stroke="black" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="m13 7l5 5m0 0l-5 5m5-5H6"/></svg>`,
        },
        {
          image: "../src/assets/blog2.jpg",
          title: "September 13 | Read in 2 minutes",
          name: "Top 10 Succulents for Your Home",
          text: "Best in hanging baskets. Prefers medium to high light.",
          link: "Read More",
          icon: `<svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" viewBox="0 0 24 24"><path fill="none" stroke="black" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="m13 7l5 5m0 0l-5 5m5-5H6"/></svg>`,
        },
        {
          image: "../src/assets/blog3.jpg",
          title: "September 15 | Read in 3 minutes",
          name: "Cacti & Succulent Care Tips",
          text: "Cacti and succulents thrive in containers and because most are..",
          link: "Read More",
          icon: `<svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" viewBox="0 0 24 24"><path fill="none" stroke="black" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="m13 7l5 5m0 0l-5 5m5-5H6"/></svg>`,
        },
        {
          image: "../src/assets/blog4.jpg",
          title: "September 15 | Read in 2 minutes",
          name: "Best Houseplants Room by Room",
          text: "The benefits of houseplants are endless. In addition to..",
          link: "Read More",
          icon: `<svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" viewBox="0 0 24 24"><path fill="none" stroke="black" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="m13 7l5 5m0 0l-5 5m5-5H6"/></svg>`,
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped></style>
