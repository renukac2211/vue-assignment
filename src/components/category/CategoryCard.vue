<script>
export default {
  components: {},
  data: () => {
    return {
      categoryHeading: "All Category",
      category: [
        {
          id: 1,
          title: "Consumer electronic",
          img: require("@/assets/images/headphone.svg"),
        },
        {
          id: 2,
          title: "Agriculture",
          img: require("@/assets/images/agriculture.png"),
        },
        {
          id: 3,
          title: "Apperel",
          img: require("@/assets/images/cloth.png"),
        },

        {
          id: 5,
          title: "Business Services",
          img: require("@/assets/images/bussiness.png"),
        },
        {
          id: 6,
          title: "Chemicals",
          img: require("@/assets/images/chemical.png"),
        },
        {
          id: 7,
          title: "Commercial Services",
          img: require("@/assets/images/commercial.png"),
        },
        {
          id: 8,
          title: "Electrical Equipment ",
          img: require("@/assets/images/electrical.png"),
        },
        {
          id: 9,
          title: "Electronic Components",
          img: require("@/assets/images/electronic.png"),
        },
        {
          id: 10,
          title: "Environment",
          img: require("@/assets/images/plant.png"),
        },
        {
          id: 11,
          title: "Fabric & Textile Raw Material",
          img: require("@/assets/images/fabric.png"),
        },
        {
          id: 12,
          title: "Fabrication Services",
          img: require("@/assets/images/scale.png"),
        },
        {
          id: 13,
          title: "Fahsion  Accessories",
          img: require("@/assets/images/cap.png"),
        },
        {
          id: 14,
          title: "Food & Beverage",
          img: require("@/assets/images/food.png"),
        },
        {
          id: 15,
          title: "Furniture",
          img: require("@/assets/images/window.png"),
        },
        {
          id: 16,
          title: "Gifts & Crafts",
          img: require("@/assets/images/gift.png"),
        },
        {
          id: 16,
          title: "Health & Medical",
          img: require("@/assets/images/hospital.png"),
        },
        {
          id: 17,
          title: "Home & Garden",
          img: require("@/assets/images/construct.png"),
        },
        {
          id: 18,
          title: "Home & Appliances",
          img: require("@/assets/images/tv.png"),
        },
        {
          id: 19,
          title: "Light & Lighting",
          img: require("@/assets/images/bulb.png"),
        },
        {
          id: 20,
          title: "Machinery",
          img: require("@/assets/images/machinery.png"),
        },
        {
          id: 21,
          title: "Material Handling",
          img: require("@/assets/images/material.png"),
        },
        {
          id: 21,
          title: "Luggage, Bags & Cases",
          img: require("@/assets/images/luggage.png"),
        },
        {
          id: 22,
          title: "Packaging & Printing",
          img: require("@/assets/images/package.png"),
        },
      ],
    };
  },
};
</script>

<template>
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
      <p>{{ item.title }}</p>
    </div>
  </div>
</template>

<style scoped>
.scrollbar-hide::-webkit-scrollbar {
  display: none;
}
</style>
