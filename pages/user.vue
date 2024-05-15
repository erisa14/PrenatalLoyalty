<template>
  <Navbar />
  <div class=" lg:w-[65%] md:w-[80%] w-[92%] mx-auto flex flex-col mt-16">
    <div class="md:flex flex-row">
      <div>
        <LeftNav/>
      </div>
      <div class="md:flex flex-col gap-6 lg:w-[51%]  mx-6 ">
        <div class="bg-[#F9ECED] px-6 pt-2 pb-28 rounded-3xl">
        <h1 class="text-[#E73B7A] text-xl font-bold tracking-tighter py-5">La tua Card</h1>
        <div class=" flex md:flex-row flex-col gap-6">
          <div class="">
          <img src="/assets/prenatal_card.png" class="rounded-3xl w-auto md:h-48 h-40" alt="Prenatal Card">
          <h2 class="-translate-y-10 text-center font-semibold text-lg tracking-wider">{{ cardNumber }}</h2>
        </div>
        <div>
          <h2 class="text-[#E73B7A] text-base tracking-tighter font-semibold">Numero Card:</h2>
          <p class=" font-semibold text-lg tracking-tight">{{ cardNumber }}</p>
          <p class="flex text-base gap-2 tracking-tighter"><h2 class="text-[#E73B7A] font-semibold">Stato:</h2>Attiva</p>
        </div>
        </div>
      </div>
        <Dati class="hidden md:flex"/>
      </div>


      <div class="grid grid-col gap-7">
        <div class="grid grid-col bg-[#EAF1FD] px-7 py-9 text-center rounded-2xl lg:w-[95%]">
          <h1 class="text-xl font-bold  text-[#E72B6F]">Passa a VIP Club
          </h1>
          <h3 class="text-sm w-3/4 tracking-tight mx-auto mt-2 font-semibold">Scopri tutti i vantaggi che ti aspettano</h3>
          <Carousel :autoplay="8000" :wrap-around="true" :items-to-show="1" @after-change="updateActiveSlide"
            v-model="activeSlide" class="-mx-10 mt-4">
            <Slide v-for="(quote, index) in quotes" :key="index">
              <div class="carousel-content bg-[white]" :class="{ 'active-quote': index === activeSlide }"
                v-html="quote"></div>
            </Slide>
            <template #addons>
                <Navigation /> 
              <Pagination />
            </template>
          </Carousel>
          <a href="/user1" type="button"
            class="bg-[#E72B6F] self-center mx-auto py-2 px-6 text-base text-white rounded-full mt-8">ACQUISTA VIP
            CARD</a>
        </div>
        <profileCompletato />
        <Dati class="md:hidden flex "/>
        <div class="grid grid-col px-9 pt-4 rounded-3xl border border-gray-300 gap-6 lg:w-[95%]">
          <h1 class="text-[#E82770] text-xl font-semibold">Invita un amico</h1>
          <div class=" flex flex-col -space-y-3 ">
            <p class="text-sm w-2/3 tracking-tight leading-4  -translate-y-3  ">Condividi i link con un tuo amico e ricevi uno sconto di 10
              euro.</p>
            <a href="#" class="underline  text-sm ">Scopri di piú</a>
          </div>
          <div class="flex flex-row">
            <input type="text" :value="link" readonly
              class="border border-1  py-3 rounded-l-md w-full font-light text-lg text-gray-300">
            <button @click="copyLink" class="bg-[#E82770] p-3 rounded-2xl rounded-l-none "><svg class="h-6 w-6 text-white" width="20"
                height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none"
                stroke-linecap="round" stroke-linejoin="round">
                <path stroke="none" d="M0 0h24v24H0z" />
                <rect x="8" y="8" width="12" height="12" rx="2" />
                <path d="M16 8v-2a2 2 0 0 0 -2 -2h-8a2 2 0 0 0 -2 2v8a2 2 0 0 0 2 2h2" />
              </svg>
            </button>
          </div>
          <div class="bg-[#E82770] text-white flex flex-row  rounded-full mt-2 mb-4 px-8  py-2  mx-auto">
            <svg class="h-6 w-6 mx-auto" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"
              stroke-linecap="round" stroke-linejoin="round">
              <circle cx="18" cy="5" r="3" />
              <circle cx="6" cy="12" r="3" />
              <circle cx="18" cy="19" r="3" />
              <line x1="8.59" y1="13.51" x2="15.42" y2="17.49" />
              <line x1="15.41" y1="6.51" x2="8.59" y2="10.49" />
            </svg>
            <button @click="shareLink" class="text-lg mx-auto">CONDIVIDI</button>
          </div>
        </div>
      </div>

    </div>
    <Vantaggi class="ml-72" />
    <HappyBox />
  </div>
  <Footer></Footer>
</template>
<style>
.carousel-content {
  font-size: 14px;
  color: black;
  width: 75%;
  height: max-content;
  border: 2px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  transition: box-shadow 0.3s ease-out;
  padding-top: 9%;
  padding-bottom: 9%;
  padding-inline: 11%;
  border-radius: 0.5rem !important;
}

.carousel-slide-active {
  border-radius: 15% !important;
}
.carousel__prev {
  color: #636062;
  width: 40px;
}
.carousel__next {
  color: #E82770;
  width: 40px;
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
  background-color: #2C5C89;
}
.carousel__icon:hover {
  color: #E82770;
}
.carousel__icon.isActive {
  color: #E82770;
}
</style>
<script>
import { defineComponent, ref } from 'vue'
import { Carousel, Pagination, Slide, Navigation } from 'vue3-carousel'
import 'vue3-carousel/dist/carousel.css'
export default defineComponent({
  name: 'MyCarousel',
  name: 'LinkComponent',
  name: 'ShareButtonComponent',
  components: {
    Carousel,
    Slide,
    Pagination,
    Navigation,
  },
  setup() {
    const link = ref('http://localhost:3000/');
    const copyLink = () => {
      navigator.clipboard.writeText(link.value)
        .then(() => {
          console.log('Link copied to clipboard');
        })
        .catch(err => {
          console.error('Failed to copy link: ', err);
        });
    };
    return {
      link,
      copyLink,
      cardNumber: 6666691002556,
    };
  },
  data() {
    return {
      quotes: [
        'Accedi a <span class="font-bold">promozini in anteprima</span> e a <span class="font-bold">promo personalizzate </span> sui tuoi interessi',
        'Accedi a <span class="font-bold">promozini in anteprima</span> e a <span class="font-bold">promo personalizzate </span> sui tuoi interessi',
      ],
      activeSlide: 0,
    };
  },
  methods: {
    updateActiveSlide(index) {
      this.activeSlide = index;
    },
    shareLink() {
      const link = 'http://localhost:3000/';
      const message = `Check out this link: ${link}`;
      const encodedMessage = encodeURIComponent(message);
      const shareUrl = `https://wa.me/?text=${encodedMessage}`;
      window.open(shareUrl, '_blank');
    },
  }
})
</script>