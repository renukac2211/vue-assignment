<script>
import CategoryCard from "../components/category/CategoryCard.vue";

export default {
  name: "HomePage",
  components: {
    CategoryCard,
  },
  data: () => {
    return {
      category: [
        {
          id: 1,
          title: "Facilities",
          img: require("@/assets/images/library.png"),
        },
        {
          id: 2,
          title: "Logistics",
          img: require("@/assets/images/logistic.png"),
        },
      ],
    };
  },

  methods: {},
};
</script>

<template>
  <div>
    <div>
      <div class="mt-5 text-lg">Recent</div>
      <div class="w-full flex flex-wrap gap-4 justify-center mt-5">
        <div
          class="rounded-lg bg-[#F5F5F5] w-32 min-w-[8rem] flex flex-col gap-2 hover:shadow-xl transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-110 cursor-pointer p-4"
          v-for="item in category"
          :key="item.id"
        >
          <div
            @click="
              $router.push({
                name: 'Facilities',
              })
            "
          >
            <img
              :src="item.img"
              alt="Brand Logo"
              class="flex justify-center items-center w-10 h-10 mx-auto"
            />
          </div>
          <div class="text-sm">
            <p>{{ item.title }}t</p>
          </div>
        </div>
      </div>
    </div>
    <!-- About me -->
    <div class="mt-5 text-lg">All Category</div>
    <div class="w-full flex flex-wrap gap-4 justify-center mt-5">
      <CategoryCard />
    </div>

    <!-- About counter -->

    <!-- About counter -->
    <!--  <div class="container mx-auto"></div> -->
  </div>
</template>

<style scoped></style>
