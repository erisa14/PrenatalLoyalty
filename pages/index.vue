<template>
  <div class="mx-auto">
    <nav>
      <Navbar></Navbar>
    </nav>


    <figure class="relative mx-auto top-5 ">

      <img class="rounded-3xl lg:w-[65%] md:w-[80%] w-[90%] md:h-auto h-[53vh] mx-auto md:object-cover object-cover filter brightness-50 md:fill-none md:brightness-100" src="/assets/indexImage.jpg" alt="image description" style="object-position: 32% 50%;">
      <figcaption class="absolute self-center flex flex-col lg:space-y-5 lg:w-[43%]  lg:right-10 lg:top-14  md:w-[45%] md:right-0 md:top-12 md:space-y-1 top-14 w-[90%] space-y-4  align-middle  justify-center text-white">
        <h1 class="lg:text-5xl lg:w-2/5 lg:self-start lg:text-left md:text-xl md:w-4/5 md:self-start md:text-left w-[55%] text-4xl self-center text-center  font-semibold">Entra nel club di Prénatal</h1>
        <p class="lg:w-2/4 lg:text-left lg:self-start lg:text-lg lg:tracking-tight lg:leading-5 md:text-left md:self-start md:tracking-tight md:w-[81%] md:text-sm md:leading-4 w-[85%] tracking-tight justify-center self-center leading-5">Registrati gratuitamente per un mondo di promozioni dedicate,
          o acquista una VIP Card per accedere a tutti i vantaggi aggiuntivi.</p>
        <a href="#" class="lg:self-start lg:py-2 lg:text-lg  md:px-4 md:py-2 md:text-base md:mt-3 md:self-start md:mb-2 px-6 py-2 rounded-3xl self-center text-white bg-[#e82770]" type="button">ACCEDI
          O REGISTRATI</a>
        <h5 class="lg:text-left lg:text-sm md:text-left md:text-xs text-xs text-center top-4">Hai perso la tua card? <a href="#" class="underline">Recupera il codice</a></h5>
      </figcaption>

    </figure>



    <div class="md:w-[80%] lg:w-[60%] w-[95%] mx-auto">
      <div class="flex lg:flex-row py-3 flex-col justify-evenly lg:gap-9 md:mt-12  lg:pt-20 px-5">
        <div class="lg:w-[60%] bg-white  flex flex-col justify-start lg:mt-7 items-center w-[98%]">
          <div class="">
            <h1 class="mb-2 lg:text-4xl text-2xl w-[60%] md:w-[30%] lg:w-full font-semibold  tracking-tight text-[#e82770]" style="color: #e82770;">I vantaggi di
              entrare nel Club</h1>
            <p class="mb-3 font-thin leading-5 md:leading-6 md:text-lg">Registrati subito per vivere una esperienza di acquisto
              sempre
              piú personalizzata e in linea con le tue esigenze.</p>
          </div>
          <div class="lg:inline-block inline-flex gap-2 relative lg:top-24 lg:ml-20 top-3 md:top-0 mb-16">
            <img class="rounded-xl lg:absolute drop-shadow-xl w-36 h-auto lg:w-[90%] lg:z-10 lg:rotate-12 lg:skew-y-6 top-24 lg:-translate-x-20"
              src="/assets/clubCard.png" alt="Prenatal vip club" />
            <img class="rounded-xl drop-shadow-xl w-36 h-auto lg:w-[90%] lg:-translate-y-3 sm:z-0 lg:-rotate-12  lg:-skew-y-6" src="/assets/pcard.png"
              alt="Prenatal card" />
            
          </div>
        </div>


        <div class="md:top-0 md:-translate-y-16">

          <swiper
    :modules="modules"
    :loop="true"
        :slides-per-view="slidesPerView"
        @slideChange="onSlideChange"
        @swiper="onSwiper"
        :draggable="true"
        :pagination="{
      clickable: true,
      
    }"  
  >
    <swiper-slide>  
       <div class="w-[97%] lg:w-[98%] md:w-[96%] rounded-xl text-center mt-6">
          <h1 class="bg-[#e82770] text-xl lg:text-2xl font-sans font-semibold text-white text-center p-7 rounded-t-3xl">Prénatal
            Card
          </h1>
          <div class="flow-root p-5 text-left shadow bg-[#ffedee] rounded-b-3xl">
            <ul class="divide-y divide-white text-[15px] md:tracking-wide md:leading-5 lg:text-lg tracking-tight lg:tracking-tight lg:leading-5 font-sans font-semibold text-[#e82770]">
              <li></li>
              <li class="flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="#297860" class="w-[18px] h-[18px]">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>
                Sarai informato in anteprima sulle promozioni
              </li>
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="#297860" class="w-[18px] h-[18px]">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>Promozioni personalizzate per te
              </li>
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="#297860" class="w-[18px] h-[18px]">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>Sconto di benvenuto
              </li>
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="#297860" class="w-[18px] h-[18px]">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>Sconto speciale in occasione del compleanno di tuo figlio/a
              </li>
              <li class="flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="#297860" class=" w-[18px] h-[18px]">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>Offerte extra dai nostri brand partner
              </li>
              <li></li>
            </ul>
            <ul class="divide-y divide-white text-[15px] md:tracking-wide md:leading-5 lg:text-lg lg:tracking-tight lg:leading-5 tracking-tight font-sans font-light" style="color: #909090;">
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="lg:w-6 lg:h-6 w-[18px] h-[18px]">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M6 18 18 6M6 6l12 12" />
                  </svg></span>Sconti a partire dal -30%
              </li>
              <li class=" flex p-2 items-center ">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="lg:w-6 lg:h-6 w-[18px] h-[18px]">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M6 18 18 6M6 6l12 12" />
                  </svg></span>
                Sconti a partire dal 30% su abbigliamento e arredo letto a marchio Prénatal
              </li>
              <li class=" flex p-2 items-center">
                <span>
                  <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="lg:w-6 lg:h-6 w-[18px] h-[18px]">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M6 18 18 6M6 6l12 12" />
                  </svg></span>
                Sconti a partire dal 10% sui marchi Nike, Adidas, Nike Jordan, Vans, Converse, New Era e Puma
              </li>
              <li class=" flex px-3 py-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="lg:w-6 lg:h-6 w-[18px] h-[18px]">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M6 18 18 6M6 6l12 12" />
                  </svg></span>Spedizione gratuita per ordini online*
              </li>
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="lg:w-6 lg:h-6 w-[18px] h-[18px]">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M6 18 18 6M6 6l12 12" />
                  </svg></span>
                Servizio di personal shopper
              </li>

              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="lg:w-6 lg:h-6 w-[18px] h-[18px]">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M6 18 18 6M6 6l12 12" />
                  </svg></span>
                Accesso all'esclusivo webinar di genitorialità
              </li>
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="lg:w-6 lg:h-6 w-[18px] h-[18px]">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M6 18 18 6M6 6l12 12" />
                  </svg></span>
                Tantissimi vantaggi su una selezione di pannolini
              </li>
              <li></li>
            </ul>
            <h1 class="text-[#e82770] text-2xl font-sans lg:font-bold font-semibold text-center px-7 lg:py-10 pt-8 pb-16">GRATIS</h1>


          </div>
          <div class="flex flex-col gap-7 px-16 -translate-y-1/4">
            <a href="#" class="button lg:py-3 py-2 rounded-3xl top-10 text-white text-lg bg-[#e82770]">REGISTRATI SUBITO</a>
            <a href="#" class="underline text-gray-500 self-center lg:text-base text-sm font-thin">Regolamento Prénatal Card</a>
          </div>
        </div></swiper-slide>
        <swiper-slide> 
        <div class="w-[97%] lg:w-[98%] md:w-[96%] rounded-xl mt-6">
          <div
            class=" overflow-auto flex flex-col justify-center text-center lg:p-5 bg-[#dddddd] text-black rounded-full md:w-[120px] md:h-[120px] absolute rotate-12 md:translate-x-56 lg:translate-x-[255px] z-10 lg:-translate-y-3  md:-translate-y-6 translate-x-64  w-[85px] h-[85px]">
            <h2 class=" text-xs">risparmia</h2>
            <h1 class="text-[#3e5884] md:text-3xl text-sm leading-4 md:font-semibold lg:font-bold">215€</h1>
            <h3 class="lg:font-light text-xs  leading-3">in media <br>ogni anno*</h3>
          </div>
          <div class=" font-sans font-semibold text-white px-7 lg:py-4 md:py-4 py-5 rounded-t-3xl bg-[#3e5884]">
            <h1 class="lg:text-2xl text-lg">Prénatal VIP Card</h1>
            <h5 class="text-[#cddfc5] lg:text-base text-xs md:text-base">12 mesi di sconti esclusivi</h5>
          </div>
          <div class="flow-root p-5 text-left shadow text-[#e82770] bg-[#eaf1fd] rounded-b-3xl">
            <ul class="divide-y divide-white text-[15px] lg:text-lg lg:tracking-tight lg:leading-5  tracking-tight md:tracking-wide md:leading-5 font-sans font-semibold">
              <li></li>
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="#297860" class="w-[18px] h-[18px]">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>
                Sarai informato in anteprima sulle promozioni
              </li>
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="#297860" class="w-[18px] h-[18px]">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>Promozioni personalizzate per te
              </li>
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="#297860" class="w-[18px] h-[18px]">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>Sconto di benvenuto
              </li>
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="#297860" class="w-[18px] h-[18px]">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>Sconto speciale in occasione del compleanno di tuo figlio/a
              </li>
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="#297860" class="w-[18px] h-[18px]">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>Offerte extra dai nostri brand partner
              </li>
              <li class=" flex px-2 py-3 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="#297860" class=" w-[18px] h-[18px]">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>Sconti a partire dal -30%
              </li>
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="#297860" class="w-[18px] h-[18px]">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>Sconti a partire dal 30% su abbigliamento e arredo letto a marchio Prénatal
              </li>
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="#297860" class="w-[18px] h-[18px]">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>Sconti a partire dal 10% sui marchi Nike, Adidas, Nike Jordan, Vans, Converse, New Era e
                Puma
              </li>
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="#297860" class="w-[18px] h-[18px]">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>Spedizione gratuita per ordini online*
              </li>
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="#297860" class="w-[18px] h-[18px]">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>Servizio di personal shopper
              </li>

              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="#297860" class=" w-[18px] h-[18px]">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>Accesso all'esclusivo webinar di genitorialità
              </li>
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="#297860" class="w-[18px] h-[18px]">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>Tantissimi vantaggi su una selezione di pannolini
              </li>
              <li></li>
            </ul>
            <div class="flex flex-col justify-between gap-3 py-5">
              <h1 class="text-[#e82770] text-2xl font-sans lg:font-bold font-semibold text-center  rounded-t-xl">30 €/anno</h1>
              <a href="#" class="text-center underline text-[#e82770] font-sans lg:text-lg text-base">Scopri tutti i vantaggi della
                VIP
                Card</a>
            </div>

          </div>
          <div class="flex flex-col gap-7 px-12 -translate-y-1/4">
            <a href="#" type="button"
              class="button lg:py-3 py-2 px-2 rounded-3xl text-center text-white lg:text-lg  bg-[#e82770]">ACQUISTA
              LA TUA VIP CARD</a>
            <a href="#" class="underline text-gray-500 self-center lg:text-base text-sm font-thin">Regolamento VIP Card</a>
          </div>
        </div>
        </swiper-slide>
    <div class="swiper-pagination " slot="pagination"></div>
  </swiper>

        </div>
      </div>
      <h5 class="hidden lg:block text-right text-sm font-light -translate-y-16">*Sconto medio ottenuto dai clienti con VIP Card nel 2023
      </h5>

    </div>

    <VipReasones/>



    <figure class="relative mx-auto  grid  mt-10 md:hidden">
      <img src="/assets/parental_skills.png" alt="image" class="w-[92%] h-[72vh] mx-auto filter rounded-3xl" >
      <figcaption
        class="absolute py-10 px-10 grid grid-col gap-5 text-lg self-center mt-36">
        <h1 class="text-xl  text-[#e82770]">Parental Skills at Work</h1>
        <p class="tracking-tighter text-sm leading-4">Se sei un cliente VIP, accedi gratuitamente al webinar
          legato alla genitorialità.
          Un percorso preparato per te con partners autorevoli per riscoprire come le skills genitoriali possono
          dare una marcia in più in famiglia e nella professione.</p>
        <a class="bg-[#e82770] text-sm font-light w-[140px] text-center  py-2 rounded-full text-white">ACCEDI SUBITO
        </a>
      </figcaption>
    </figure>
    <figure class=" md:relative md:mx-auto  md:grid lg:w-[62%] md:w-[80%]  md:mt-10 hidden">
      <img src="https://card.prenatal.com/_ipx/f_webp/images/parental-skills.png" alt="image" class=" lg:w-full lg:h-[30vh]   mx-auto filter rounded-3xl" >
      <figcaption
        class="absolute self-center lg:px-4 grid grid-col lg:gap-5 md:gap-3 lg:w-[47%]  lg:right-12 md:w-[50%] md:right-3  ">
        <h1 class="lg:text-3xl font-semibold  text-[#e82770]">Parental Skills at Work</h1>
        <p class="lg:tracking-tight lg:leading-5 lg:text-lg md:text-sm md:leading-4 md:font-light">Se sei un cliente VIP, accedi gratuitamente al webinar
          legato alla genitorialità.
          Un percorso preparato per te con partners autorevoli per riscoprire come le skills genitoriali possono
          dare una marcia in più in famiglia e nella professione.</p>
        <a class="bg-[#e82770] lg:text-lg font-light lg:w-[170px] md:w-[140px] text-center  py-2 rounded-full text-white">ACCEDI SUBITO
        </a>
      </figcaption>
    </figure>



    <happyBox class=" mt-10"/>

    <div class="lg:w-[62%] md:w-[80%] mt-16 mx-auto">

    <div class="relative sm:pt-8 sm:px-4 px-6">
      <h1 class=" text-[#E72B6F] lg:text-2xl lg:text-start md:text-start md:text-xl text-center  font-semibold ">Altri vantaggi esclusivi</h1>
      <div class="flex lg:flex-row md:flex-row flex-col lg:justify-between md:gap-1 lg:gap-0 gap-5 ">
        <p class="translate-y-4 lg:text-base md:text-left md:text-sm from-neutral-700 text-center ">Scopri le offerte attive in questo momento con i nostri
          partner selezionati, tutte riservate ai soli clienti registrati</p>
        <a href="#" type="button"
          class=" text-[#E72B6F] lg:text-lg lg:text-right lg:right-24 lg:px-5 lg:py-2 lg:-translate-y-3 md:px-1 md:-translate-y-5 border-[1px]  text-center border-[#E72B6F] py-3 rounded-full font-medium">SCOPRI
          DI PIÙ</a>
      </div>
    </div>

    <Carousel :wrap-around="true" :items-to-show="itemsToShow"  @after-change="updateActiveSlide"
      v-model="activeSlide" class=" mx-auto mt-10 mb-20">
      <Slide v-for="(image, index) in images" :key="index">
        <img :src="image.url" class="carousel-image  rounded-3xl" :class="{ 'active-image': index === activeSlide }"
          alt="Carousel image">
      </Slide>

      <template #addons>
        <Navigation/>
        <Pagination />
      </template>
    </Carousel>

</div>
    <div class="bg-[#f2d5d6] text-center p-5">
      <p class="text-[#e82770] text-xl font-semibold mx-4">Hai giá una card?
        <a>
          <button class="bg-[#e82770] font-normal text-white text-lg mx-3 rounded-3xl px-7 py-2">ACCEDI</button>
        </a>
      </p>
    </div>
    <footer class="bottom-0">
      <Footer></Footer>
    </footer>
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
      images: [
        { url: 'https://www.picclickimg.com/WDIAAOSwD1Rlo6gT/CODICE-VOUCHER-COUPON-PHOTOSI-20EURO-GIFT-PROMOZIONALE-SCONTO.webp' },
        { url: 'https://www.richmonditalia.it/wp-content/themes/yootheme/cache/Elty-c9c630f5.jpeg' },
        { url: 'https://www.bitrefill.com/primg/w350h212/lastminute_com-belgium-holiday-flight-_-hotel-packages-belgium.webp' },
        { url: 'https://storage.googleapis.com/prg-loyalty.appspot.com/media/93/CLINIQUE_IMMAGINE-ANTEPRIMA.png' },
        { url: 'https://storage.googleapis.com/prg-loyalty.appspot.com/media/102/img-logo---595x422px.jpg' },
      ],
      activeSlide: 0,
      itemsToShow: 5, 
      slidesPerView:2,
    };
  },
  methods: {
    updateActiveSlide(index) {
      this.activeSlide = index;
    },
    updateItemsToShow() {
      const screenWidth = window.innerWidth;
      if (screenWidth<1000) {
        this.itemsToShow=1;
      }

      else{
        this.itemsToShow = 5; 

      }
    },

    updateSlide(){
      const screenWidth = window.innerWidth;
      if (screenWidth <= 640) { 
        this.slidesPerView = 1.2; 
      } else {
        this.slidesPerView = 2; 
      }
      
    },
  },
  mounted() {
    window.addEventListener('resize', this.updateItemsToShow);
    this.updateItemsToShow(); 
    this.updateSlide();
    window.addEventListener('resize', this.updateSlide);
  },
  beforeUnmount() {
    window.removeEventListener('resize', this.updateItemsToShow);
    window.removeEventListener('resize', this.updateSlide);

  },
});
</script>

<style>

@import 'swiper/swiper-bundle.css';

.swiper-pagination-bullet-active {
  background: blue; 
}
.active-image {
  transform: scale(1.7);
  z-index: 1;
  border-radius: 0.5rem !important;
}



.carousel__prev {
  color: #636062;
}

.carousel__next {
  color: #E82770;
}

.carousel-image {
  border-radius: 0.5rem !important;
  width: 85%;
}

@media (max-width: 640px) {
 .carousel-image {
    width: 30%; 
    border-radius: 0.5rem!important; 
    overflow-x: hidden;
    
  }
 .active-image {
    width: 70%;
    z-index: 1;
    border-radius: 0.5rem!important; 
   
  }
 .responsive-screen{
    width: 80%;
  }
 .carousel__prev {
    display: none;
  }

 .carousel__next {
    display: none;
  }
}


@media (max-width: 1000px) {
  .carousel-image {
    width: 60%; 
    border-radius: 0.5rem!important; 
    overflow-x: hidden;
    
  }
 
 .carousel__prev {
    display: none;
  }

 .carousel__next {
    display: none;
  }
}


.carousel__slide--sliding {
  transition: 0.5s;
}

.carousel__slide {
  opacity: 0.9;
  transform: rotateY(-20deg) scale(0.9);
}


.carousel__pagination-button::before,
.carousel__pagination-button::after {
  content: none;
}

.carousel__pagination-button {
  width: 12px;
  height: 12px;
  border-radius: 50%;
  background-color: #ccc;
  border: none;
  padding: 0;
  margin: 0 5px;
}

.carousel__pagination-button--active {
  background-color: blue;
}

.carousel__icon:hover {
  color: #e82770;
}

.carousel__icon.isActive {
  color: #e82770;
}

</style>
