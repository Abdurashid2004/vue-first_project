<template>
  <div v-for="(item, index) in plants" :key="index" class="p-2">
    <img :src="item.image" class="w-[258px] h-[300px]" alt="" />
    <h2 class="pt-4 text-base">{{ item.name }}</h2>
    <p class="font-bold text-green-500">{{ item.price }}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      plants: [
        {
          name: "Barberton Daisy",
          price: "$119.00",
          image: "../src/assets/product1 (2).jpg",
        },
        {
          name: "Angel Wing Begonia",
          price: "$169.00",
          image: "../src/assets/foto2.jpg",
        },
        {
          name: "African Violet",
          price: "$199.00",
          image: "../src/assets/foto3.jpg",
        },
        {
          name: "Beach Spider Lily",
          price: "$129.00",
          image: "../src/assets/foto4.jpg",
        },
        {
          name: "Blushing Bromeliad",
          price: "$139.00",
          image: "../src/assets/foto5.jpg",
        },
        {
          name: "Aluminum Plant",
          price: "$179.00",
          image: "../src/assets/foto6.jpg",
        },
        {
          name: "Bird's Nest Fern",
          price: "$99.00",
          image: "../src/assets/foto7.jpg",
        },
        {
          name: "Broadleaf Lady Palm",
          price: "$59.00",
          image: "../src/assets/foto8.jpg",
        },
        {
          name: "Chinese Evergreen",
          price: "$39.00",
          image: "../src/assets/foto9.jpg",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped></style>
