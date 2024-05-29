<template>
  <div class="flex flex-wrap mb-32 mt-32">
    <!-- Blog Cards -->
    <div class="grid md:grid-cols-3 flex-1 w-[204px]">
      <div v-for="(item, index) in blogs" :key="index" class="flex-col ">
        <div class="w-full overflow-hidden ">
          <img :src="item.image" alt="" class="object-cover pl-4" />
        </div>
        <div class="mt-4">
          <h3 class="text-lg font-lg font-bold">{{ item.name }}</h3>
          <p class="text-gray-700 w-[204px]">{{ item.text }}</p>
        </div>
      </div>
    </div>

    <!-- Newsletter Form -->
    <div class="mt-8 md:mt-0 md:w-1/4 flex flex-col">
      <h3 class="text-xl font-semibold mb-4">
        Would you like to join newsletters?
      </h3>
      <div class="flex max-w-xs">
        <input
          type="text"
          placeholder="enter your email address..."
          class="mb-2 p-2 w-full border border-gray-300 flex-1 rounded-l-lg"
        />
        <button
          class="px-6 bg-green-600 text-white hover:bg-green-500 rounded-r-lg"
          style="height: 42px"
        >
          Join
        </button>
      </div>
      <p class="mt-4 text-gray-600">
        We usually post offers and challenges in newsletter. We’re your online
        houseplant destination. We offer a wide range of houseplants and
      </p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      blogs: [
        {
          image: "../src/assets/blog5.jpg",
          name: "Garden Care",
          text: "We are an online plant shop offering a wide range of cheap and trendy plants.",
        },
        {
          image: "../src/assets/blog6.jpg",
          name: "Plant Renovation",
          text: "We are an online plant shop offering a wide range of cheap and trendy plants.",
        },
        {
          image: "../src/assets/blog5.jpg",
          name: "Watering Garden",
          text: "We are an online plant shop offering a wide range of cheap and trendy plants.",
        },
      ],
    };
  },
};
</script>

<style scoped>
/* Add any additional styling here */
</style>
