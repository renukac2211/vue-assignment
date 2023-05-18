<script>
export default {
  name: "ProductList",
  components: {},
  data: () => {
    return {};
  },

  methods: {},
};
</script>

<template>
  <div class="w-full flex justify-center px-6">
    <div
      class="text-sm font-medium text-center text-gray-500 border-b border-gray-200 dark:text-gray-400 dark:border-gray-700 w-full flex justify-center items-center"
    >
      <ul class="flex flex-wrap -mb-px">
        <li class="mr-2">
          <a
            href="#"
            class="inline-block p-4 border-b-2 border-transparent rounded-t-lg hover:text-gray-600 hover:border-gray-300 dark:hover:text-gray-300"
            >All</a
          >
        </li>
        <li class="mr-2">
          <a
            href="#"
            class="inline-block p-4 text-blue-600 border-b-2 border-blue-600 rounded-t-lg active dark:text-blue-500 dark:border-blue-500"
            aria-current="page"
            >Aucion</a
          >
        </li>
        <li class="mr-2">
          <a
            href="#"
            class="inline-block p-4 border-b-2 border-transparent rounded-t-lg hover:text-gray-600 hover:border-gray-300 dark:hover:text-gray-300"
            >Buynow</a
          >
        </li>
      </ul>
    </div>
  </div>
</template>

<style scoped></style>
