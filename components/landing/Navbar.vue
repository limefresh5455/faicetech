<script setup>
const menuitems = [
  {
    title: "Home",
    path: "#",
  },
  {
    title: "Products",
    path: "#",
  },
  {
    title: "Solutions",
    path: "#",
  },
  {
    title: "Compliance",
    path: "#",
  },
  {
    title: "About us",
    path: "#",
  },
  {
    title: "Latest...",
    path: "#",
  },
  {
    title: "Contact",
    path: "#",
  },
];

const open = ref(false);
</script>
<template>
  <LandingContainer>
   <section> 
    <header class="flex flex-col lg:flex-row items-center my-5">
      <div class="flex w-full lg:w-auto items-center">
        <a href="/" class="text-lg"
          >
          <img
        class=""
        src="~/assets/img/logo.png"
        alt=""
        loading="eager"
        format="avif"
        width="168"
        height="48"
      />
        </a>
        <div class="block lg:hidden">
          <button @click="open = !open" class="text-gray-800">
            <svg
              fill="currentColor"
              class="w-4 h-4"
              viewBox="0 0 20 20"
              xmlns="http://www.w3.org/2000/svg"
            >
              <title>Menu</title>
              <path
                v-show="open"
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M18.278 16.864a1 1 0 01-1.414 1.414l-4.829-4.828-4.828 4.828a1 1 0 01-1.414-1.414l4.828-4.829-4.828-4.828a1 1 0 011.414-1.414l4.829 4.828 4.828-4.828a1 1 0 111.414 1.414l-4.828 4.829 4.828 4.828z"
              ></path>
              <path
                v-show="!open"
                fill-rule="evenodd"
                d="M4 5h16a1 1 0 010 2H4a1 1 0 110-2zm0 6h16a1 1 0 010 2H4a1 1 0 010-2zm0 6h16a1 1 0 010 2H4a1 1 0 010-2z"
              ></path>
            </svg>
          </button>
        </div>
      </div>
      <nav
        class="w-full lg:w-auto mt-2 lg:flex lg:mt-0 ms-auto mr-20"
        :class="{ block: open, hidden: !open }"
      >
        <ul class="flex flex-col lg:flex-row lg:gap-3 themenavbar">
          <li v-for="item of menuitems">
            <a
              :href="item.path"
              class="flex font-bebas lg:px-3 py-2 text-lg uppercase font-normal text-white-theme hover:text-white-theme:hover"
            >
              {{ item.title }}
            </a>
          </li>
        </ul>
        <div class="lg:hidden flex items-center mt-3 gap-4">
          <LandingLink href="#" styleName="muted" block size="md"
            >Client Portal</LandingLink
          >
          <LandingLink href="#" size="md" block>Support</LandingLink>
        </div>
      </nav>
      <div>
        <div class="hidden lg:flex items-center gap-4">         
          <LandingLink class="btn-primary-btn font-bebas uppercase text-lg font-normal" href="#" size="md">Client Portal</LandingLink>
          <LandingLink class="btn-primary-outline-btn font-bebas uppercase text-lg font-normal" href="#" size="md">Support</LandingLink>
        </div>
      </div>
    </header>
  </section>
  </LandingContainer>
</template>
