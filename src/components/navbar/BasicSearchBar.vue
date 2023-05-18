<script>
export default {
  name: "NavBar",
  components: {},
  data: () => {
    return {
      imageUrl: require("@/assets/images/menu.png"), // Replace with your image URL
    };
  },

  methods: {},
};
</script>

<template>
  <div class="h-16">
    <input
      type="search"
      placeholder="Search Categories for insight"
      class="rounded-full border w-full"
    />

    <!-- About me -->
  </div>
</template>

<style scoped></style>
