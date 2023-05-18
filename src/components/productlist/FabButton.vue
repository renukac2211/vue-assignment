<script>
export default {
  name: "ProductList",
  components: {},
  data: () => {
    return {
      sortarrow: require("@/assets/images/sortarrow.png"),
      icon: require("@/assets/images/sort.png"),
    };
  },

  methods: {},
};
</script>

<template>
  <div>
    <div class="w-full flex justify-center items-center cursor-pointer">
      <div class="bg-[#3665F3] rounded-full flex">
        <p class="flex flex-1 px-8 py-3 text-white gap-1">
          <img :src="icon" class="w-6 h-6" />
          <span>Sort</span>
        </p>
        <p class="flex flex-1 px-8 py-3 text-white gap-1">
          <img :src="sortarrow" class="w-6 h-6" />
          <span>Filter</span>
        </p>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
