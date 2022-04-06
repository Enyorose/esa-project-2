<template>
  <div class="h-50v md:h-70v lg:h-90v">
    <!-- move this into the nav? or make a hero component -->
    <header
      class="
        w-full
        h-full
        bg-no-repeat bg-cover bg-right-bottom
        sm:bg-fixed
        flex flex-col
      "
      style="
        background-image: url('https://images.unsplash.com/photo-1598818384697-62330d600309?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=687&q=80');
      "
    >
      <TheNavBar class="sticky top-0 z-50" />
      <CtaButton />
    </header>
    <div>
      <CompanyBanner />
      <TextBox :info="textInfo" />
    </div>
  </div>
</template> 

<script setup>
const textInfo = {
  title: "Welcome!",
  text: "First a big thank you to our generous sponsors without you so many of our students would not have attended seminars and social events.  Allowing them to grow their experiences and networks providing them with so many strengths they can put towards their future.",
  img: "/assets/images/group-of-people.jpg",
  alt: "A group of people by brown trees",
};
</script>