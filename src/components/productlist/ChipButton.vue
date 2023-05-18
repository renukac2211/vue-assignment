<script>
export default {
  name: "ProductList",
  components: {},
  data: () => {
    return {};
  },

  methods: {},
};
</script>

<template>
  <div class="w-full flex overflow-x-auto scrollbar-hide py-2">
    <div class="flex justify-start md:justify-center w-full mt-2 gap-3">
      <div
        class="whitespace-nowrap px-4 cursor-pointer rounded-full flex border border-gray-300 text-gray-500 py-1 bg-[#E5E5E5] w-auto"
      >
        <router-link to="/facilities"> All </router-link>
      </div>

      <div
        class="whitespace-nowrap px-4 cursor-pointer rounded-full flex justify-center items-center border border-gray-300 text-gray-500 py-1 mr-2 bg-[#fff] w-auto"
      >
        <router-link to="/facilities"> Maintainance services </router-link>
      </div>
      <div
        class="whitespace-nowrap px-4 cursor-pointer rounded-full flex justify-center items-center border border-gray-300 text-gray-500 py-1 mr-2 bg-[#fff] w-auto"
      >
        <router-link to="/facilities"> Work wear & Uniforms</router-link>
      </div>
      <div
        class="whitespace-nowrap px-4 cursor-pointer rounded-full flex justify-center items-center border border-gray-300 py-1 mr-2 bg-[#0043FF] text-white w-auto"
      >
        View all
      </div>
    </div>
  </div>
</template>

<style scoped>
.scrollbar-hide::-webkit-scrollbar {
  display: none;
}
</style>
