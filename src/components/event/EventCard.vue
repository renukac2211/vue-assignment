<script>
export default {
  components: {},
  data: () => {
    return {
      icon: require("@/assets/images/user.png"),

      category: [
        {
          id: 1,
          title: "Requirement of 2000 Diodes at Nasik plant",
          header: "New",
          header1: "Scheduled",
          time: "Sat, 02:PM onwards",
        },
        {
          id: 1,
          title: "Requirement of 2000 Diodes at Nasik plant",
          header: "New",
          header1: "Scheduled",
          time: "Sat, 02:PM onwards",
        },
        {
          id: 1,
          title: "Requirement of 2000 Diodes at Nasik plant",
          header: "New",
          header1: "Scheduled",
          time: "Sat, 02:PM onwards",
        },
      ],
    };
  },
};
</script>

<template>
  <div
    class="flex flex-col bg-white shadow-2xl p-3 w-96 rounded"
    v-for="item in category"
    :key="item.id"
  >
    <div class="flex flex-col justify-start items-start gap-2">
      <div class="flex gap-2">
        <div
          class="bg-[#2398F6] text-white rounded px-3 py-1 text-xs font-medium"
        >
          New
        </div>
        <div
          class="bg-[#2398F6] text-white rounded px-3 py-1 text-xs font-medium"
        >
          Scheduled
        </div>
      </div>

      <div class="flex justify-between w-full">
        <div class="text-sm w-60 flex text-start font-semibold">
          Requirement of 2000 Diodes at Nasik plant
        </div>
        <div class="flex flex-col text-xs">
          <span
            class="bg-[#2398F6] text-white rounded-t-2xl px-3 py-[2px] text-xs font-medium"
          >
            Nov
          </span>
          <span class="text-[#2398F6]"> 12</span>
        </div>
      </div>

      <div class="text-sm text-[#3B3B3B]">Sat, 02:PM onwards</div>
      <div class="flex justify-center items-center gap-2">
        <div class="bg-[#C4C4C4] rounded-full w-8 h-8"></div>
        <div class="flex flex-col items-start">
          <p class="text-[#1A1A1A] text-sm">Andrew Smith</p>
          <p class="text-[#585858] text-sm">Global foundries</p>
        </div>
      </div>
      <div
        class="text-[#1DDDC7] text-sm flex justify-center items-center gap-2"
      >
        <div class="bg-white rounded-full p-2 shadow-lg">
          <img :src="icon" class="w-4 h-4" />
        </div>
        <span> one on one</span>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
