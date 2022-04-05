<template>
  <div class="sm:w-90v mx-auto p-6 md:p-8 bg-gray-100 shadow-lg opacity-70">
    <h2 class="text-md md:text-base lg:text-2xl mb-5 text-center">
      Our Gold Sponsors
    </h2>
    <div class="flex flex-wrap justify-between">
      <article v-for="link in links" :key="link.id">
        <img class="h-10 md:h-16 lg:h-20" :src="link.path" />
      </article>
    </div>
  </div>
</template>

<script setup>
const links = [
  {
    path: "../assets/images/allnorth.jpg",
    alt: "This is a photo of the allnorth photo.",
  },
  {
    path: "../assets/images/dwb.jpg",
    alt: "This is a photo of the dwb photo.",
  },
  {
    path: "../assets/images/gairns.png",
    alt: "This is a photo of the dwb photo.",
  },
  {
    path: "../assets/images/mcelhanney.png",
    alt: "This is a photo of the mcelhanney photo.",
  },
  {
    path: "../assets/images/unbc.jpeg",
    alt: "This is a photo of the unbc photo.",
  },
];
</script>