<template>
  <div class="bg-gray-100 shadow-lg w-90v mx-auto rounded-md mt-6">
    <h2 class="pt-4 pl-4 text-lg md:text-xl lg:text-2xl">
      {{ props.box.title }}
    </h2>
    <div class="flex justify-around mt-6">
      <Card v-for="card in cards" :key="card.id" :info="card" />
    </div>
  </div>
</template>

<script setup>
const props = defineProps({
  box: {
    type: Object,
  },
});

const cards = [
  {
    img: "/assets/images/bailey-edwards.jpg",
    alt: "Photo of student bailey edwards",
    text: "ESA has been a fantastic learning experience for me! My time as a part of the executive team has catalyzed growth both academically and professionally. I have made new connections with students of all years and been introduced to a few mentors that have helped ... See more",
    author: "Bailey Edwards",
  },
  {
    img: "/assets/images/jeff-watson.JPG",
    alt: "Photo of student bailey edwards",
    text: "ESA has been a fantastic learning experience for me! My time as a part of the executive team has catalyzed growth both academically and professionally.",
    author: "Jeff Watson",
  },
  {
    img: "/assets/images/jessica-watson.jpg",
    alt: "Photo of student bailey edwards",
    text: "ESA has been a fantastic learning experience for me! My time as a part of the executive team has catalyzed growth both academically and professionally. I have made new connections with students",
    author: "Jessica Watson",
  },
];
</script>
