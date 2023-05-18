<script>
import FacilityCard from "@/components/facility/FacilityCard.vue";
export default {
  name: "Facilities",
  components: {
    FacilityCard,
  },
  data: () => {
    return {};
  },

  methods: {},
};
</script>

<template>
  <div class="mt-3">
    <!-- About me -->
    <div>
      <FacilityCard />
    </div>
  </div>
</template>

<style scoped></style>
