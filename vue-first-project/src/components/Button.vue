<template>
  <div class="mb-[120px]">
    <div v-for="(item, index) in buttons" :key="index" class="">
      <div class="float-right flex flex-row">
        <div>
          <button
            class="px-4 py-2 text-xl rounded-lg border border-gray-500 hover:text-white hover:bg-green-500 mx-2 text-center"
            v-html="item.button"
          ></button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      buttons: [
        {
          button: `<svg class="button-icon" width="8" height="28" viewBox="0 0 8 12" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M1.375 0.75C1.375 0.75 6.625 3.858 6.625 6C6.625 8.14125 1.375 11.25 1.375 11.25" stroke="#3D3D3D" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
</svg>`,
        },
        { button: "4" },
        { button: "3" },
        { button: "2" },
        { button: "1" },
      ],
    };
  },
};
</script>

<style scoped>
.button-icon {
  display: inline-block;
  vertical-align: middle;
  margin: auto 0;
  height: 1.5em; /* Adjust the height as needed */
}
</style>
