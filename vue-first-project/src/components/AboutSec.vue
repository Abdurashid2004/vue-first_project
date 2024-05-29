<template>
  <div class="grid grid-cols-1 sm:grid-cols-2 gap-12 mb-11">
    <div v-for="(item, index) in items" :key="index" class="flex items-center p-4">
      <img :src="item.image" alt="" class="w-[300px] h-[350px]" />
      <div class="flex flex-col ml-4">
        <h2 class="text-lg font-bold mb-2 w-[180px]">{{ item.name }}</h2>
        <div class="flex flex-col justify-between">
          <p class="text-gray-700 mb-4">{{ item.text }}</p>
          <button class="px-4 py-2 bg-green-500 text-white rounded-lg hover:bg-green-700 flex items-center w-[130px]">
            {{ item.click }}
            <span v-html="item.icon" class="ml-2"></span>
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          image: "../src/assets/product1 (2).jpg",
          name: "SUMMER CACTUS & SUCCULENTS",
          text: "We are an online plant shop offering a wide range of cheap and trendy plants",
          click: "Find More",
          icon: `<svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" viewBox="0 0 24 24"><path fill="none" stroke="white" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="m13 7l5 5m0 0l-5 5m5-5H6"/></svg>`
        },
        {
          image: "../src/assets/product1 (2).jpg",
          name: "SUMMER CACTUS & SUCCULENTS",
          text: "We are an online plant shop offering a wide range of cheap and trendy plants",
          click: "Find More",
          icon: `<svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" viewBox="0 0 24 24"><path fill="none" stroke="white" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="m13 7l5 5m0 0l-5 5m5-5H6"/></svg>`
        }
      ]
    };
  }
};
</script>

<style scoped>
.h2 {
  width: 180px;
}
</style>
