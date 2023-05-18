<script>
import EventCard from "../components/event/EventCard.vue";
import ActionBox from "../components/home/ActionBox.vue";
import Slider from "../components/home/Slider.vue";
import CategoryCard from "../components/category/CategoryCard.vue";
import ProductListCard from "../components/productlist/ProductListCard.vue";

export default {
  name: "HomePage",
  components: {
    EventCard,
    ActionBox,
    Slider,
    CategoryCard,
    ProductListCard,
  },
  data: () => {
    return {};
  },

  methods: {},
};
</script>

<template>
  <div>
    <!-- About me -->

    <div class="container mx-auto">
      <ActionBox />
      <Slider />
      <div>
        <div class="flex justify-between items-center mb-3 px-2">
          <p class="text-lg font-bold">Explore Popular Categories</p>
          <router-link
            to="/category"
            class="text-sm text-[#4D79EB] cursor-pointer"
            >View All
          </router-link>
        </div>
        <!-- 
        <div class="w-full flex flex-wrap gap-4">
          <CategoryCard />
        </div> -->

        <div
          class="flex justify-center gap-3 w-full pl-32 overflow-x-auto overflow-y-hidden scrollbar-hide"
        >
          <CategoryCard />
        </div>
      </div>

      <div class="mt-5">
        <div class="flex justify-between items-center">
          <p class="text-lg font-bold">Trending Auctions</p>
          <router-link
            to="/productlisting"
            class="text-sm text-[#4D79EB] cursor-pointer"
            >View All
          </router-link>
        </div>
        <p class="text-start text-sm">
          See what's popular across thousands of Auctions
        </p>
        <div class="border-dashed border-b border-[#4D79EB] mt-3"></div>

        <div
          class="flex justify-center gap-3 w-full overflow-x-auto overflow-y-hidden scrollbar-hide"
        >
          <ProductListCard />
        </div>
        <div class="border-dashed border-b border-[#4D79EB] mt-3"></div>
      </div>

      <div class="mt-5">
        <div class="flex justify-between items-center">
          <p class="text-lg font-bold">Featured products</p>
          <router-link
            to="/productlisting"
            class="text-sm text-[#4D79EB] cursor-pointer"
            >View All
          </router-link>
        </div>
        <p class="text-start text-sm">
          See what's popular across thousands of Products
        </p>
        <div class="border-dashed border-b border-[#4D79EB] mt-3"></div>
        <div
          class="flex justify-center gap-3 w-full overflow-x-auto overflow-y-hidden scrollbar-hide"
        >
          <ProductListCard />
        </div>
        <div class="border-dashed border-b border-[#4D79EB] mt-3"></div>
      </div>

      <div class="mt-5">
        <div class="flex justify-between items-center">
          <p class="text-lg font-bold">Featured Services</p>
        </div>
        <p class="text-start text-sm">
          See what's popular across thousands of Products
        </p>
        <div class="border-dashed border-b border-[#4D79EB] mt-3"></div>

        <div
          class="flex justify-center gap-3 w-full overflow-x-auto overflow-y-hidden scrollbar-hide"
        >
          <ProductListCard />
        </div>
        <div class="border-dashed border-b border-[#4D79EB] mt-3"></div>
      </div>
      <div class="mt-5">
        <div class="flex justify-between items-center">
          <p class="text-lg font-bold">Featured Event</p>
        </div>
        <p class="text-start text-sm">
          See what's popular across thousands of Products
        </p>
        <div class="border-dashed border-b border-[#4D79EB] mt-3"></div>

        <div
          class="flex justify-center gap-3 w-full overflow-x-auto overflow-y-hidden scrollbar-hide mt-10 pb-5"
        >
          <EventCard />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.scrollbar-hide::-webkit-scrollbar {
  display: none;
}
</style>
