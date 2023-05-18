<script>
export default {
  components: {},
  data: () => {
    return {
      categoryHeading: "All Category",
      category: [
        {
          id: 1,
          title: "MENS SEIKO KENETIC TITANIUM 100M WRIST WATCH! No Reserve!",
          img: require("@/assets/images/view.png"),
          price: "Price: $ 100",
          timeLeft: "Time Left",
          time: "1d 23h 59m",
          bids: "5 bids",
          shipping: "+$11.60 shipping",
        },
        {
          id: 1,
          title: "MENS SEIKO KENETIC TITANIUM 100M WRIST WATCH! No Reserve!",
          img: require("@/assets/images/view.png"),
          price: "Price: $ 100",
          timeLeft: "Time Left",
          time: "1d 23h 59m",
          bids: "5 bids",
          shipping: "+$11.60 shipping",
        },
        {
          id: 1,
          title: "MENS SEIKO KENETIC TITANIUM 100M WRIST WATCH! No Reserve!",
          img: require("@/assets/images/view.png"),
          price: "Price: $ 100",
          timeLeft: "Time Left",
          time: "1d 23h 59m",
          bids: "5 bids",
          shipping: "+$11.60 shipping",
        },
        {
          id: 1,
          title: "MENS SEIKO KENETIC TITANIUM 100M WRIST WATCH! No Reserve!",
          img: require("@/assets/images/view.png"),
          price: "Price: $ 100",
          timeLeft: "Time Left",
          time: "1d 23h 59m",
          bids: "5 bids",
          shipping: "+$11.60 shipping",
        },
        {
          id: 1,
          title: "MENS SEIKO KENETIC TITANIUM 100M WRIST WATCH! No Reserve!",
          img: require("@/assets/images/view.png"),
          price: "Price: $ 100",
          timeLeft: "Time Left",
          time: "1d 23h 59m",
          bids: "5 bids",
          shipping: "+$11.60 shipping",
        },
        {
          id: 1,
          title: "MENS SEIKO KENETIC TITANIUM 100M WRIST WATCH! No Reserve!",
          img: require("@/assets/images/view.png"),
          price: "Price: $ 100",
          timeLeft: "Time Left",
          time: "1d 23h 59m",
          bids: "5 bids",
          shipping: "+$11.60 shipping",
        },
        {
          id: 1,
          title: "MENS SEIKO KENETIC TITANIUM 100M WRIST WATCH! No Reserve!",
          img: require("@/assets/images/view.png"),
          price: "Price: $ 100",
          timeLeft: "Time Left",
          time: "1d 23h 59m",
          bids: "5 bids",
          shipping: "+$11.60 shipping",
        },
        {
          id: 1,
          title: "MENS SEIKO KENETIC TITANIUM 100M WRIST WATCH! No Reserve!",
          img: require("@/assets/images/view.png"),
          price: "Price: $ 100",
          timeLeft: "Time Left",
          time: "1d 23h 59m",
          bids: "5 bids",
          shipping: "+$11.60 shipping",
        },
      ],
    };
  },
};
</script>

<template>
  <div
    class="flex flex-col bg-white lg:p-4 mt-5"
    v-for="item in category"
    :key="item.id"
  >
    <div>
      <img
        :src="category[0].img"
        alt="category[0].title"
        class="w-40 h-48 object-cover rounded-sm lg:w-60 lg:h-48"
      />
    </div>
    <div class="text-sm flex justify-start items-start flex-col">
      <p class="text-start lg:w-60 w-40 capitalize">
        MENS SEIKO KENETIC TITANIUM 100M WRIST WATCH! No Reserve!
      </p>
      <p class="text-lg">Price: $ 100</p>
      <div class="flex flex-col gap-1 justify-start items-start">
        <p class="text-[#707070] text-xs">Time Left</p>
        <p class="text-[#F40000] text-sm">1d 23h 59m</p>
        <p class="text-[#707070] text-xs">5 bids</p>
        <p class="text-[#707070] text-xs">+$11.60 shipping</p>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
