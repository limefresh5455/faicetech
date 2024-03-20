<template>
  <div class="w-full bg-theme-black py-0.5">
    <div class="max-w-screen-xl mx-auto px-5">
      <LandingNavbar></LandingNavbar>
    </div>
  </div>
  <div>
    <slot></slot>
  </div>
  <LandingFooter></LandingFooter>
</template>
