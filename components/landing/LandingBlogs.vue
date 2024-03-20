<script setup>
definePageMeta({
  layout: "landing",
});

const TeamImg1 = "https://raw.githubusercontent.com/limefresh5455/faicetech/main/assets/img/blog2.png";
const TeamImg2 = "https://raw.githubusercontent.com/limefresh5455/faicetech/main/assets/img/blog3.png";
const TeamImg3 = "https://raw.githubusercontent.com/limefresh5455/faicetech/main/assets/img/blog4.png";
const TeamImg4 = "https://raw.githubusercontent.com/limefresh5455/faicetech/main/assets/img/blog1.png";

const blogsTeam = [
  {
    title: "How great Content helps drive success in Marketplace",
    discription: "Majority of peole will work in jobs that don’t exist today.",
    date:'02 Feb 2024',
    readmore:"READ MORE",
    avatar: {
      src: TeamImg1,
      width: 315,
      height: 231,
    },
  },
  {
    title: "8 Rules of Thumb in UI Design",
    discription: "Majority of peole will work in jobs that don’t exist today.",
    date:'02 Feb 2024',
    readmore:"READ MORE",
    avatar: {
      src: TeamImg2,
      width: 315,
      height: 231,
    },
  },
  {
    title: "Cyber Attack: Is the 'Big One' coming soon in 2022",
    discription: "Majority of peole will work in jobs that don’t exist today.",
    date:'02 Feb 2024',
    readmore:"READ MORE",
    avatar: {
      src: TeamImg3,
      width: 315,
      height: 231,
    },
  },
  {
    title: "Why do chief security officers leave jobs so often?",
    discription: "Majority of peole will work in jobs that don’t exist today.",
    date:'02 Feb 2024',
    readmore:"READ MORE",
    avatar: {
      src: TeamImg4,
      width: 315,
      height: 231,
    },
  },
];
</script>

<template>
   <div class="BlogSection">
  <LandingContainer>
    <div class="flex flex-col gap-3 mx-auto max-w-4xl mt-16 mb-16">
                    <div class="text-center">
                      <span class="text-small-blue">BLOG</span>
                      <h3 class="mb-7 mt-2">Read our Latest Blog</h3>
                      <p>Amet nisl suscipit adipiscing bibendum est ultricies integer. Tincidunt arcu non sodales neque
                        sodales. Sed felis eget velit aliquet sagittis id. Viverra mauris in aliquam sem.
                      </p>
                    </div>
    </div>
    <div class="grid md:grid-cols-4 gap-5 mx-auto w-11/12">
      <div v-for="item of blogsTeam" class="group">
        <div class="w-full aspect-square">
          <img
            :src="item.avatar.src"
            :width="item.avatar.width"
            :height="item.avatar.height"
            format="avif"
            alt="Team"
            class="w-full h-full object-cover rounded transition group-hover:-translate-y-1 group-hover:shadow-xl"
          />
        </div>
        <div class="blogContWrap">
          <div class="blogContMask bg-[url('~/assets/img/blogboxcurve-bg-black.png')]"></div>
              <div class="mt-4 text-center relative px-7">
                <h5>{{ item.title }}</h5>
                <p>{{ item.discription }}</p>
              </div>
              <div class="flex justify-between relative px-7">
                  <span class="text-white">{{ item.date }}</span>
                  <span class="flex items-center">
                    <LandingLink
                      href="#"
                      class="px-0 py-0 uppercase linkblue bg-transparent hover:bg-transparent"
                      target="_blank"
                      rel="noopener"
                      >{{ item.readmore }}                       
                    </LandingLink> 
                    <svg width="16" height="13" viewBox="0 0 16 13" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path d="M1.33334 6.5H14.6667M14.6667 6.5L9.66668 1.5M14.6667 6.5L9.66668 11.5" stroke="#3ECEF6" stroke-width="1.66667" stroke-linecap="round" stroke-linejoin="round"/>
                        </svg>
                  </span>
              </div>
        </div>
      </div>
     
    </div>
    <div class="mt-12 text-center">
        <LandingLink
          href="#"
          class="btn-primary-btn font-bebas text-lg uppercase font-bold px-6 py-4"
          target="_blank"
          rel="noopener"
          >View All Blogs</LandingLink
        >       
      </div>
  </LandingContainer>
</div>



</template>
