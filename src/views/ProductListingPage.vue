<script>
import ProductListCard from "../components/productlist/ProductListCard.vue";
import FabButton from "../components/productlist/FabButton.vue";
import Tab from "../components/productlist/Tab.vue";
import ChipButton from "../components/productlist/ChipButton.vue";
export default {
  name: "ProductList",
  components: {
    ProductListCard,
    FabButton,
    Tab,
    ChipButton,
  },
  data: () => {
    return {
      icon: require("@/assets/images/sort.png"),
      searchIcon: require("@/assets/images/search.svg"),
      sortarrow: require("@/assets/images/sortarrow.png"),
      listIcon: require("@/assets/images/list.svg"),
    };
  },

  methods: {},
};
</script>

<template>
  <div class="mt-3">
    <div>Facility management > Maintainanance services > level 3</div>
    <div class="w-full">
      <ChipButton />
    </div>
    <div class="border-b border-[#E5E5E5] mx-6 my-3"></div>

    <div class="flex gap-12 lg:gap-52 justify-center items-center text-sm">
      <div class="text-lg">+90,000+result</div>
      <div class="flex text-sm gap-4">
        <div>
          <img :src="listIcon" class="w-6 h-6" />
        </div>
        <div>
          <img :src="searchIcon" class="w-6 h-6" />
        </div>

        <div
          class="flex justify-center items-center gap-1 text-[#0043ff] font-semibold"
        >
          <img :src="sortarrow" class="w-6 h-6" />
          <span class="text-sm"> Sort </span>
        </div>
        <div
          class="flex gap-1 font-semibold text-[#0043ff] justify-center items-center"
        >
          <img :src="icon" class="w-6 h-6" />
          <span class="text-sm"> Filter </span>
        </div>
      </div>
    </div>

    <Tab />
    <div class="w-full flex justify-center items-center flex-wrap gap-3">
      <ProductListCard />
      <div class="fixed bottom-0 right-0 mr-5 mb-5 left-0 z-50">
        <FabButton />
      </div>
    </div>
  </div>
</template>

<style scoped></style>
