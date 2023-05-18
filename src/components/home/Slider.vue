<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from "swiper/vue";

// Import Swiper styles
import "swiper/css";

import "swiper/css/pagination";
import "swiper/css/navigation";

// import required modules
import { Autoplay, Pagination, Navigation } from "swiper";

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [Autoplay, Pagination, Navigation],
    };
  },
  data: () => {
    return {
      imageUrl: require("@/assets/images/man.png"), // Replace with your image URL
    };
  },
};
</script>

<template>
  <div class="py-10 m-3">
    <swiper
      :spaceBetween="30"
      :centeredSlides="true"
      :autoplay="{
        delay: 2500,
        disableOnInteraction: false,
      }"
      :pagination="{
        clickable: true,
      }"
      :modules="modules"
      class="mySwiper rounded-md"
    >
      <swiper-slide>
        <img
          key="imageUrl"
          :src="imageUrl"
          class="object-fill w-full lg:h-96 h-44"
        />
        <!-- <img
          className="object-fill w-full lg:h-96 h-44"
          src="https://cdn.pixabay.com/photo/2022/03/20/15/40/nature-7081138__340.jpg"
          alt="image slide 1"
        /> -->
      </swiper-slide>
      <swiper-slide>
        <img
          className="object-fill w-full lg:h-96 h-44"
          src="https://cdn.pixabay.com/photo/2022/07/24/17/55/wind-energy-7342177__340.jpg"
          alt="image slide 2"
        />
      </swiper-slide>
      <swiper-slide>
        <img
          className="object-fill w-full lg:h-96 h-44"
          src="https://cdn.pixabay.com/photo/2022/07/26/03/35/jogger-7344979__340.jpg"
          alt="image slide 3"
        />
      </swiper-slide>
    </swiper>
  </div>
</template>
