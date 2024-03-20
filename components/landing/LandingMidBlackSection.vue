<script setup>
const BenefitsBtm = [
  {
    title: "HONEST",
    description:
      "We will not allow automated decisions to be made with a legal or similar effect, without their appropriate human verification.",
   
  },
  {
    title: "unique",
    description:
      "We will not allow automated decisions to be made with a legal or similar effect, without their appropriate human verification.",
    
  },
  {
    title: "SECURE",
    description:
      "We will not allow automated decisions to be made with a legal or similar effect, without their appropriate human verification.",
    
  },
  {
    title: "unique",
    description:
      "We will not allow automated decisions to be made with a legal or similar effect, without their appropriate human verification.",
   
  },
  {
    title: "ethical",
    description:
      "We will not allow automated decisions to be made with a legal or similar effect, without their appropriate human verification.",
    
  },
];
</script>
<template>
    <!-- Top section -->
  <div class="MidBlackTwoSectionWrap">

   <div class="MidBlackTwoSection bg-[url('~/assets/img/move-forward-bg.png')]">
    <div class="flex items-center h-full">  
        <div class="flex-auto"></div>
        <div class="flex-auto w-12">
          <div class="MidBlackRight">
                    <h3>MOVE FORWARD WITH CONFIDENCE:</h3>
                    <p>We place compliance and privacy at the forefront of our facial recognition
                    technology, ensuring both cutting-edge solutions and unwavering protection
                    of individual rights and data security.</p>
                    <p>
                    We are fully committed to the UK General Data Protection Regulation (GDPR)
                    and are happy to discuss all our policies and processes.</p>
          </div>
        </div>
      </div>
    </div>

    <!-- bottom section -->
    <div class="MidBlackTwoSectionBtm bg-[url('~/assets/img/benefit-bottom-bg.png')]">
      <div class="flex items-center justify-center h-full"> 
          <div class="MidBlackBottom">
            <span class="text-small-green">Benefits</span>
                    <h3>BENEFITS OF WORKING WITH FAICETECH</h3>
                    <p>Our proprietary technology and process enables us to deliver a high level of accuracy whilst utilising bank level security to ensure data is stored and accessed securely. Unlike others, our privacy and security by design paradigm means we are the only UK service provider that has always met or exceeded all expectations.</p>
          </div>
       
      </div>

      <div class="flex flex-wrap justify-center gap-6 w-11/12 mx-auto mt-20" >
        <div v-for="item of BenefitsBtm" class="flex justify-center benfitbox">    
          <span class="markSign">
            <img
            class=""
            src="~/assets/img/mark-right.png"
            alt=""
           
            format="avif"
            width="61"
            height="60"
          />
      </span>    
          <div>
            <h4>{{ item.title }}</h4>
            <p>
              {{ item.description }}
            </p>
          </div>
        </div>
       </div>
      
    </div>









  </div>
</template>
