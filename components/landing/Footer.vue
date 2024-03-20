<template>
<footer class="footersection bg-[url('~/assets/img/footer-bg.png')]">
  <div class="grid md:grid-cols-4 gap-10 mx-auto w-10/12 mt-12">
      <div class="w-full">
        <span>
            <img
            class=""
            src="~/assets/img/Faice-Icon_Blue _footer.png"
            alt=""
            loading="eager"
            format="avif"
            width="84"
            height="132"
          />
          </span>
          <p class="text-white text-left my-5">Cutting edge machine learning technology, meets privacy by design</p>
          <span>
            <img
            class=""
            src="~/assets/img/axis.png"
            alt=""
            loading="eager"
            format="avif"
            width="122"
            height="94"
          />
          </span>
      </div>

      <div class="w-full ml-20">
        <ul class="font-normal">
        <h6 class="mb-5">Products</h6>
        <li><a href="">FaiceAlert</a></li>
        <li><a href="">FaiceMatch</a></li>
        <li><a href="">FaiceAccess</a></li>
        </ul>
      </div>
  
      <div class="w-full">
        <ul>
          <h6 class="mb-5">Use Cases</h6>
          <li><a href="#">Retail Risk & Loss Prevention</a></li>
          <li><a href="#">Responsible Gambling & Gaming</a></li>
          <li><a href="#">Facial Recognition for Access Control</a></li>
          <li><a href="#">Student Campuses</a></li>
          <li><a href="#">Public Transport</a></li>
          <li><a href="#">Critical Infrastructure</a></li>
          <li><a href="#">Mining Safety and Security</a></li>
          <li><a href="#">Stadiums & Mass Public Venues</a></li>
          <li><a href="#">Healthcare & GPs</a></li>
        </ul>
      </div>

      <div class="w-full ml-20">
        <ul>
          <li><a href="#" class="font-bold">Case Studies</a></li>
          <li><a href="#" class="font-bold">Company</a></li>
          <li><a href="#" class="font-bold">InfoSec</a></li>
          <li><a href="#" class="font-bold">News</a></li>
          <li><a href="#" class="font-bold">Events</a></li>
          <li><a href="#" class="font-bold">Press Releases</a></li>
          <li><a href="#" class="font-bold">Case Studies</a></li>
          <li><a href="#" class="font-bold">White Papers</a></li>
          <li><a href="#" class="font-bold">Thought Leadership</a></li>
          <li><a href="#" class="font-bold">Version Control</a></li>
          <li><a href="#" class="font-bold">Documentation</a></li>
          <li><a href="#" class="font-bold">Terms</a></li>
          <li><a href="#" class="font-bold">Privacy Policy</a></li>
          <li><a href="#" class="font-bold">FAQs</a></li>
          <li><a href="#" class="font-bold">Contact</a></li>
        </ul>
      </div>

  </div>

  <div class="grid md:grid-cols-4 gap-10 mx-auto w-10/12 mt-12">
    <div class="w-full">    
        <h6 class="mb-5">Head Office</h6>
       <p class="text-footer text-left my-5">
        292 Hale Road, Hale Barns, Altrincham, WA15 8SP, 
        United Kingdom
       </p>       
    </div>
    <div class="w-full">    
        <h6 class="mb-5">Request a demo</h6>
       <p class="text-footer text-left my-5">
        <span class="flex items-center">
          <span> <img
            class=""
            src="~/assets/img/USA-flag.png"
            alt=""
            loading="eager"
            format="avif"
            width="21"
            height="16"
          />
          </span>
          <p class="text-footer ml-3">+44 (0) 20 3011 4000</p>
        </span>
     
        <span class="flex items-center">
          <span> <img
            class=""
            src="~/assets/img/UK-flag.png"
            alt=""
            loading="eager"
            format="avif"
            width="21"
            height="16"
          />
          </span>
          <p class="text-footer ml-3">+1 (213) 205-2200</p>
        </span>
        <p class="mt-5 text-left">
        <LandingLink
          href="mailto:info@faicetech.com"
          class="ps-0 py-0 bg-transparent hover:bg-transparent"
          target="_blank"
          rel="noopener"
          >info@faicetech.com</LandingLink
        >       
        </p>
       </p>       
    </div>   
  </div>
  <div class="footerinfo mx-auto w-10/12 mt-12">  
   
  
    <p class="text-left text-footer mt-1 flex justify-between">
      <span class="flex">
       <small class="text-sm">Find Us On:</small>
      <a
        href="#"
        target="_blank"
        rel="noopener"
        class="hover:underline"
      >
      <span> <img
            class="ml-5"
            src="~/assets/img/footerlinkedIn.png"
            alt=""
            loading="eager"
            format="avif"
            width="99"
            height="24"
          />
          </span>
      </a>
    </span>
    <span>
     <p class="text-footer">
      © {{ new Date().getFullYear() }} FaiceTech Ltd All Rights Reserved.
    </p>
  </span>
    </p>
  </div>
    
</footer>
</template>
