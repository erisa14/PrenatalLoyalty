<template>
    <div class=" lg:w-[63%] md:w-[80%] w-[92%] flex flex-col gap-4 mt-16">
        <h1 class="text-[#E72B6F] lg:text-4xl lg:text-left text-center text-xl font-bold ">Altri vantaggi esclusivi</h1>
        <h3 class="lg:text-[17px] lg:text-left  lg:self-start lg:leading-normal self-center text-center tracking-tight">Scopri le offerte attive in questo momento con i nostri partner selezionati, tutte riservate ai soli clienti registrati</h3>
      
        <div class="lg:flex gap-5 hidden">
        <img src="https://www.bitrefill.com/primg/w350h212/lastminute_com-belgium-holiday-flight-_-hotel-packages-belgium.webp" class="vantaggi-image" alt="">
        <img src="https://www.richmonditalia.it/wp-content/themes/yootheme/cache/Elty-c9c630f5.jpeg" class="vantaggi-image border-2 border-gray-300" alt="">
        <img src="https://www.picclickimg.com/WDIAAOSwD1Rlo6gT/CODICE-VOUCHER-COUPON-PHOTOSI-20EURO-GIFT-PROMOZIONALE-SCONTO.webp" class="vantaggi-image" alt="">
        <img alt="" class="vantaggi-image" src="https://storage.googleapis.com/prg-loyalty.appspot.com/media/102/img-logo---595x422px.jpg">
        <img src="https://storage.googleapis.com/prg-loyalty.appspot.com/media/93/CLINIQUE_IMMAGINE-ANTEPRIMA.png" class="vantaggi-image" alt="">
      </div>
   

        <div class="w-[92%] lg:hidden mx-auto">
            <swiper
    :modules="modules"
    :loop="true"
        :slides-per-view="2"
        :space-between="0"
        @slideChange="onSlideChange"
        @swiper="onSwiper"
        :draggable="true"
        :pagination="{
      clickable: true,
      
    }"  
  >
    <swiper-slide>
        
            <img src="https://www.bitrefill.com/primg/w350h212/lastminute_com-belgium-holiday-flight-_-hotel-packages-belgium.webp" class="swiper-img" alt="">

      
        </swiper-slide>
        <swiper-slide>
 <img src="https://www.richmonditalia.it/wp-content/themes/yootheme/cache/Elty-c9c630f5.jpeg" class="swiper-img border-2 border-gray-300" alt=""></swiper-slide>
 <swiper-slide>
<img src="https://www.picclickimg.com/WDIAAOSwD1Rlo6gT/CODICE-VOUCHER-COUPON-PHOTOSI-20EURO-GIFT-PROMOZIONALE-SCONTO.webp" class="swiper-img" alt=""></swiper-slide>
<swiper-slide>
  <img alt=""  src="https://storage.googleapis.com/prg-loyalty.appspot.com/media/102/img-logo---595x422px.jpg" class="swiper-img"></swiper-slide>
  <swiper-slide>
 <img src="https://storage.googleapis.com/prg-loyalty.appspot.com/media/93/CLINIQUE_IMMAGINE-ANTEPRIMA.png" alt="" class="swiper-img"></swiper-slide>
    <div class="mt-10 " slot="pagination"></div>

    </swiper>
        </div>
        <button class=" border border-[#E72B6F] text-[#E72B6F] rounded-3xl lg:w-[180px] lg:py-2 w-[87%] py-2 mx-auto text-xl mb-5">SCOPRI DI PIÚ</button>
    </div>
</template>


<script>
import { defineComponent, onMounted, onBeforeUnmount } from 'vue';
import { Carousel, Slide, Navigation } from 'vue3-carousel';
import { Swiper, SwiperSlide } from 'swiper/vue';

import 'swiper/swiper-bundle.css';
import 'swiper/css';
import 'swiper/css/pagination'; 
import 'vue3-carousel/dist/carousel.css';
import { Pagination } from 'swiper/modules';

export default defineComponent({
  name: 'MyCarousel',
  components: {
    Carousel,
    Slide,
    Pagination,
    Navigation,
    Swiper,
      SwiperSlide,
  },
  setup() {
     
      return {
        modules:[Pagination],
      };
    },
  data() {
    return {
      slidesPerView:2,
    };
  },
  methods: {
    updateActiveSlide(index) {
      this.activeSlide = index;
    },
   

}
});
</script>

<style>
@import 'swiper/swiper-bundle.css';

.vantaggi-image {
    width: 22%;
    height: auto;
    border-radius: 0.5rem;
  }

 .swiper-img{
    margin-right: 10px;
    width: 90%;
    height: 100px;
    border-radius: 0.5rem;
 }
</style>
