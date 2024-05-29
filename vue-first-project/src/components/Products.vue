<template>
  <div class="mb-[90px]">
    <div class="flex justify-between items-center">
      <div class="flex justify-between items-center gap-16 text-sm">
        <h3 class=" text-base hover:text-green-500 hover:border-b-2 border-green-500 pb-2">
          All Plants
        </h3>
        <h3 class="text-base hover:text-green-500 hover:border-b-2 border-green-500 pb-2">
          New Arrivals
        </h3>
        <h3 class=" text-base hover:text-green-500 hover:border-b-2 border-green-500 pb-2">
          Sale
        </h3>
      </div>
      <div class="items-center flex gap-2">
        <span>Short by: Default sorting </span>
        <span
          ><svg
            width="16"
            height="16"
            viewBox="0 0 16 16"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M12.6666 5.66667L7.99998 10.3333L3.33331 5.66667"
              stroke="#3D3D3D"
              stroke-width="1.5"
              stroke-linecap="round"
              stroke-linejoin="round"
            />
          </svg>
        </span>
      </div>
    </div>

    <div class="grid grid-cols-3 gap-24">
      <ProductCard v-for="item in 1" />
    </div>
  </div>
</template>

<script>
import ProductCard from "./ProductCard.vue";

export default {
  components: { ProductCard },
  setup() {
    return {};
  },
};
</script>

<style lang="scss" scoped></style>
