<script>
export default {
  components: {},
  data: () => {
    return {
      category: [
        {
          id: 1,
          title: "Request Anything",
        },
        {
          id: 2,
          title: "Create Event",
        },
        {
          id: 3,
          title: "Auction item",
        },
      ],
    };
  },
};
</script>

<template>
  <div class="w-full mt-7">
    <!-- About me -->
    <div class="w-full">
      <div class="flex justify-center items-center gap-2 cursor-pointer">
        <div class="lg:p-6 lg:px-10 bg-[#C4C4C4] p-4">Request</div>
        <div class="lg:p-6 lg:px-10 bg-[#C4C4C4] p-4">Create</div>
        <div class="lg:p-6 lg:px-10 bg-[#C4C4C4] p-4">Auction</div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
