<template>
  <div class="MidBlackTtestimonialWrap">
    <div class="MidBlackTtestimonial">   
      <Carousel>
        <Slide v-for="slide in items" :key="slide.title">
          <div class="carousel__item">
            <p>{{ slide.description }}</p>
            <div class="flex mt-10 gap-5">
              <span class="clientPic">               
                <img
                  class=""
                  :src="slide.image"
                  alt=""
                  format="avif"
                  width="50"
                  height="50"
                />              
              </span> 
              <div class="profileBox">
                <h5>{{ slide.name }}</h5>
                <span class="clienProfile">{{ slide.title }}</span>
              </div>
            </div>
          </div>
        </Slide>
        <template #addons>         
          <Pagination />
        </template>
      </Carousel>
    </div>
  </div>
</template>

<script>
import { defineComponent } from 'vue'
import { Carousel, Navigation, Pagination, Slide } from 'vue3-carousel'

import 'vue3-carousel/dist/carousel.css'

export default defineComponent({
  name: 'Basic',
  components: {
    Carousel,
    Slide,
    Pagination,
    Navigation,
  },
  data () {
    return {
      items: [
        { 
          title: 'Freelance Designer',
          name: 'Mila mcscuba',
          description: `In hac habitasse platea dictumst. Curabitur condimentum porta lacus, eget facilisis enim vu/putate id. Vivamus et mi et urna congue ullamcorper at ac nis/. Praesent ac u/lamcorper ipsum. Donec tempor tempor augue, at facilisis neque suscipit ut. Vivamus euismod, nunc ac viverra gravida, tortor risus sagittis nisl, at egestas metus diam a magna.`,
          image: '/assets/img/mila.png',

        },
        {
          title: 'Freelance Developer',
          name: 'Olivia John',
          description: `In hac habitasse platea dictumst. Curabitur condimentum porta lacus, eget facilisis enim vu/putate id. Vivamus et mi et urna congue ullamcorper at ac nis/. Praesent ac u/lamcorper ipsum. Donec tempor tempor augue, at facilisis neque suscipit ut. Vivamus euismod, nunc ac viverra gravida, tortor risus sagittis nisl, at egestas metus diam a magna.`,
          image: '/assets/img/mila.png' 
        },
        { 
          title: 'Business Analyst',
          name: 'Amelia',
          description: `In hac habitasse platea dictumst. Curabitur condimentum porta lacus, eget facilisis enim vu/putate id. Vivamus et mi et urna congue ullamcorper at ac nis/. Praesent ac u/lamcorper ipsum. Donec tempor tempor augue, at facilisis neque suscipit ut. Vivamus euismod, nunc ac viverra gravida, tortor risus sagittis nisl, at egestas metus diam a magna.`,
          image: '/assets/img/mila.png' 
        },
      ],
    }
  }
})
</script>

<style>
ol.carousel__pagination {
    justify-content: flex-start;
    margin-top: 25px;
    gap: 10px;
  }
.carousel__pagination-button {background: #d9d9d9;width: 15px;height: 15px;display: block;padding: 0;border-radius: 50%;margin-right: 5px;}
button.carousel__pagination-button.carousel__pagination-button--active {background: #3ECDF5 !important;}
.carousel__pagination-button::after{content:none;}
</style>
