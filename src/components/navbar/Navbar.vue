<script>
import SearchBar from "./SearchBar.vue";
import BasicSearchBar from "./BasicSearchBar.vue";

export default {
  name: "NavBar",
  components: {
    SearchBar,
    BasicSearchBar,
  },
  methods: {
    goBack() {
      this.$router.go(-1); // Navigate back to the previous page
    },
  },

  mounted() {
    const currentUrl = this.$route.path;
    console.log(currentUrl); // Output the current URL
  },
  data: () => {
    return {
      icon: require("@/assets/images/sort.png"),
      imageUrl: require("@/assets/images/menu.png"), // Replace with your image URL
      imageUrl1: require("@/assets/images/back.png"),
    };
  },
};
</script>

<template>
  <div class="bg-white shadow-lg h-16">
    <div
      class="flex justify-start items-center lg:px-16 px-3"
      v-if="$route.path === '/facilities'"
    >
      <div @click="goBack" class="cursor-pointer">
        <img key="imageUrl1" :src="imageUrl1" class="h-6 w-6 mt-4 m-1" />
      </div>
      <div class="mt-2 w-full flex justify-center items-center">
        <p class="flex justify-center items-center mt-3 text-lg">
          Facility Management
        </p>
      </div>
    </div>

    <div
      class="flex justify-start items-center lg:px-16 px-3"
      v-if="$route.path === '/category'"
    >
      <div class="mb-3 cursor-pointer" @click="goBack">
        <img key="imageUrl1" :src="imageUrl1" class="h-6 w-6" />
      </div>
      <div class="mt-2 w-full flex justify-center items-center">
        <div class="lg:w-1/2"><BasicSearchBar /></div>
      </div>
    </div>
    <!-- About me -->
    <div
      class="flex justify-start items-center lg:px-24 px-3"
      v-if="$route.path === '/' || $route.path === '/productlisting'"
    >
      <div
        class="cursor-pointer"
        @click="
          $router.push({
            name: 'Homepage',
          })
        "
      >
        <img key="imageUrl" :src="imageUrl" class="h-6 w-6 mt-4 m-1" />
      </div>

      <div class="flex w-full lg:justify-end gap-2">
        <div class="lg:w-1/2 w-full">
          <SearchBar />
        </div>
        <div
          class="flex justify-center items-center mt-4 gap-2 font-bold text-[#0043ff] cursor-pointer"
        >
          <img :src="icon" class="w-6 h-6" />
          <span class="text-sm">Filter</span>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
