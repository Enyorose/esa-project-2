<template>
  <section class="w-90v flex flex-col md:flex-row mx-auto mt-7 md:items-center">
    <div>
      <h2 class="text-lg font-semibold md:text-xl lg:text-3xl">
        {{ props.info.title }}
      </h2>
      <p class="lg:text-xl sm:w-3/4 my-2">{{ props.info.text }}</p>
    </div>
    <img
      class="md:h-64 rounded-md"
      :src="props.info.img"
      :alt="props.info.alt"
    />
  </section>
</template>

<script setup>
const props = defineProps({
  info: {
    type: Object,
  },
});
</script>