<template>
  <div class="">
    <img class="h-64" :src="props.info.img" :alt="props.info.alt" />
    <p class="w-20v pt-3">{{ props.info.text }}</p>
    <figcaption class="pt-2">{{ props.info.author }}</figcaption>
  </div>
</template>

<script setup>
const props = defineProps({
  info: {
    type: Object,
  },
});
</script>