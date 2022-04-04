<template>
  <div class="h-50v md:h-70v lg:h-90v">
    <header
      class="
        w-full
        h-full
        bg-no-repeat bg-cover bg-right-bottom bg-fixed
        flex flex-col
      "
      style="
        background-image: url('https://images.unsplash.com/photo-1598818384697-62330d600309?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=687&q=80');
      "
    >
      <TheNavBar class="sticky top-0 z-50" />
      <section class="my-auto ml-3">
        <h1 class="font-body text-xl md:text-3xl lg:text-5xl xl:text-7xls">
          Help us shape the future
        </h1>
        <CtaButton />
      </section>
    </header>
    <div class="h-4/5"></div>
  </div>
</template> 