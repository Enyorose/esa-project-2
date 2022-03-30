<template>
    <div>
    <NuxtLink
      v-for="navLink in navLinks"
      :key="navLink.id"
      :to="navLink.path"
      >{{ navLink.name }}</NuxtLink>
      </div>
</template>
<script setup>
const navLinks= [
    {
        name: 'Home',
        path: '/'
    },
    {
        name: 'Team',
        path: '/'
    },
    {
        name: 'Social',
        path: '/'
    },
    {
        name: 'Sponsor',
        path: '/'
    },
    {
        name: 'Contact',
        path: '/'
    },
    {
        name: 'Events',
        path: '/'
    }
]
</script>