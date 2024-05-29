<template>
  <div class="">
    <div class="categories w-[290px]">
      <div class="py-3">
        <h3 class="text-[18px] font-bold py-3">Categories</h3>
        <div
          v-for="(cat, index) in categories"
          :key="index"
          class="flex justify-between ml-3 gap-5 py-[10px]"
        >
          <a href="#">{{ cat.name }}</a>
          <p>({{ cat.amount }})</p>
        </div>
      </div>
      <div class="price-range">
        <h3 class="text-lg pb-3 font-bold">Price Range</h3>
        <input class="w-48" type="range" />
        <div class="flex gap-2">
          <p>Price:</p>
          <span class="text-green-400 font-bold block">$39 - $1230</span>
        </div>
        <div class="pt-2">
          <button
            class="py-2 px-6 bg-green-500 rounded-lg font-semibold text-white text-lg hover:bg-green-400"
          >
            Filter
          </button>
        </div>
      </div>
      <div class="sizes pt-4">
        <h3 class="text-[18px] font-bold py-2">Size</h3>
        <d
          iv
          v-for="(cat, index) in sizes"
          :key="index"
          class="flex justify-between ml-3 gap-5 py-[10px]"
        >
          <a href="#">{{ cat.name }}</a>
          <p>({{ cat.amount }})</p>
        </d>
      </div>
    </div>
    <div class="mt-5">
      <img
        src="../assets/Super Sale Banner.jpg "
        class="w-[390px] h-[470px]"
        alt=""
      />
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      categories: [
        { name: "House Plants", amount: 34 },
        { name: "Potter Plants", amount: 12 },
        { name: "Seeds", amount: 14 },
        { name: "Small Plants", amount: 32 },
        { name: "Flowers", amount: 19 },
        { name: "Garden Plants", amount: 92 },
        { name: "Hellowe Plants", amount: 45 },
        { name: "Lollipo jerrys", amount: 92 },
        { name: "Superset Exos", amount: 45 },
      ],
      sizes: [
        { name: "Small", amount: 234 },
        { name: "Large", amount: 127 },
        { name: "Medium", amount: 102 },
      ],
    };
  },
};
</script>

<style scoped>
input[type="range"] {
  background-color: #9a905d;
}
</style>
