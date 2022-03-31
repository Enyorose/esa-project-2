<template>
  <header class="bg-gray-100 shadow-lg flex justify-between">
    <div class="flex items-center justify-between p-4 text-gray-500">
      <div class="flex items-center">
        <svg
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
          viewBox="0 0 73 72"
          class="w-8"
        >
          <path
            d="M64.23 58.979c-5.475 6.49-13.092 10.858-21.505 12.335a36.598 36.598 0 0 1-24.482-4.263c-7.397-4.23-13.047-10.909-15.951-18.857a35.5 35.5 0 0 1 .076-24.589c2.954-7.93 8.644-14.576 16.068-18.762A36.603 36.603 0 0 1 42.943.724c8.404 1.526 15.994 5.94 21.429 12.461A35.622 35.622 0 0 1 72.65 36.37l-3.526-.036a32.158 32.158 0 0 0-7.473-20.93c-4.907-5.888-11.758-9.872-19.345-11.25a33.044 33.044 0 0 0-22.124 3.718c-6.702 3.78-11.84 9.779-14.506 16.939a32.048 32.048 0 0 0-.068 22.197c2.622 7.176 7.722 13.205 14.4 17.024A33.04 33.04 0 0 0 42.11 67.88c7.596-1.333 14.471-5.277 19.414-11.135l2.707 2.234Z"
            fill="#000"
          />
          <path
            stroke="#000"
            stroke-width="5"
            d="m21.666 43.006 14.72-16.823M33.316 25.032l9.463 8.937M55.531 22 33.977 46.183M54.246 19.671l14.72 15.245"
          />
        </svg>
        <span class="mx-2">ESA</span>
      </div>
      <div class="sm:hidden">
        <button
          @click="isOpen = !isOpen"
          type="button"
          class="
            block
            text-gray-500
            hover:text-gray-700
            focus:text-gray-700 focus:outline-none
          "
        >
          <svg
            data-prefix="fas"
            data-icon="bars"
            class="w-4 fill-current"
            role="img"
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 448 512"
          >
            <path
              fill="currentColor"
              d="M16 132h416c8.837 0 16-7.163 16-16V76c0-8.837-7.163-16-16-16H16C7.163 60 0 67.163 0 76v40c0 8.837 7.163 16 16 16zm0 160h416c8.837 0 16-7.163 16-16v-40c0-8.837-7.163-16-16-16H16c-8.837 0-16 7.163-16 16v40c0 8.837 7.163 16 16 16zm0 160h416c8.837 0 16-7.163 16-16v-40c0-8.837-7.163-16-16-16H16c-8.837 0-16 7.163-16 16v40c0 8.837 7.163 16 16 16z"
            ></path>
          </svg>
        </button>
      </div>
    </div>
    <div :class="isOpen ? 'block' : 'hidden'" class="px-2 pb-4 sm:block">
      <NuxtLink
        v-for="navLink in navLinks"
        :key="navLink.id"
        class="
          flex flex-col
          sm:flex-row
          px-2
          font-semibold
          text-gray-500
          hover:text-gray-700
          focus:text-gray-700
        "
        :to="navLink.path"
        >{{ navLink.name }}</NuxtLink
      >
    </div>
  </header>
</template>
<script setup>
const navLinks = [
  {
    name: "Home",
    path: "/",
  },
  {
    name: "Team",
    path: "/",
  },
  {
    name: "Social",
    path: "/",
  },
  {
    name: "Sponsor",
    path: "/",
  },
  {
    name: "Contact",
    path: "/",
  },
  {
    name: "Events",
    path: "/",
  },
];
</script>
<script>
export default {
  data() {
    return { isOpen: false };
  },
};
</script>