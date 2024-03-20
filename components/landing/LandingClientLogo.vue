<script setup>
definePageMeta({
  layout: "landing",
});

import logo1 from './assets/img/booths.png';
import logo2 from './assets/img/NBCS.png';
import logo3 from './assets/img/Range.png';
import logo4 from './assets/img/americangolf.png';
import logo5 from './assets/img/JD.png';

const clientlogo = [
  {   
    avatar: {
      src: logo1,    
    },
  },
  {   
    avatar: {
      src: logo2,     
    },
  },
  {  
    avatar: {
      src: logo3,     
    },
  },
  {  
  avatar: {
    src: logo4,   
  },
    },
  {  
  avatar: {
    src: logo5,   
  },
  },
];
</script>

<template>   
<LandingContainer>
    <div class="ClientlogoSection">
        <h2 class="mb-7 mt-2">Trusted by brands</h2>
    <div class="grid md:grid-cols-5 gap-10 mx-auto w-10/12 mt-12 clientlogos">
      <div v-for="item of clientlogo" class="group">
        <div class="">
          <span>
          <img
            :src="item.avatar.src"
            :width="item.avatar.width"
            :height="item.avatar.height"
            format="avif"
            alt=""
            class=""
          />
          </span>
        </div>

      </div>
     
    </div>
</div>
  </LandingContainer>
</template>
