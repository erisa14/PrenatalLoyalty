

<template>
    <div class="bg-[#F7F7F7] px-7 py-5 text-center rounded-2xl grid grid-col gap-[60px]">
        <div>
            <h1 class="text-xl font-semibold text-[#E72B6F] tracking-tight">Profilo Completato al</h1>
            <div id="app">
    <div class="circle-progress mt-10">
      <svg :width="size" :height="size" viewBox="0 0 100 100">
        <circle
          class="circle-progress__background"
          :r="radius"
          :cx="center"
          :cy="center"
          fill="none"
          stroke="#DDDDDD"
          :stroke-width="backgroundStrokeWidth"
        />
        <circle
          class="circle-progress__foreground"
          :r="radius"
          :cx="center"
          :cy="center"
          fill="none"
          stroke="#E72B6F"
          :stroke-width="foregroundStrokeWidth"
          :stroke-dasharray="circumference"
          :stroke-dashoffset="offset"
          stroke-linecap="round"
          transform="rotate(-90) translate(-100)"
        />
        <text :x="center" :y="center" text-anchor="middle" dominant-baseline="middle" font-size="25" font-weight="800">
        {{ percentage }}%
      </text>
      </svg>
    </div>
    </div>
            <span class=" text-sm mb-6 md:block hidden">7 campi compilati su 10</span>
        </div>
        <div>
            <h1 class="text-xl font-semibold text-[#E72B6F] tracking-tight">Consigli</h1>
            <Carousel :wrap-around="true" :items-to-show="1" @after-change="updateActiveSlide"
                v-model="activeSlide" class="-mx-10 mt-5">
                <Slide v-for="(quote, index) in quotes" :key="index">
                    <div class="carousel-content bg-[white]" :class="{ 'active-quote': index === activeSlide }"
                        v-html="quote"></div>
                </Slide>
                <template #addons>
                    <Navigation />
                    <Pagination />
                </template>
            </Carousel>
        </div>
        <a href="#" class="border border-[#E72B6F] rounded-full text-lg px-4 text-[#E72B6F] self-center py-2 mx-auto mt-10 w-full">COMPLETA IL PROFILO</a>
    </div>
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
  padding-inline: 9%;
  border-radius: 0.5rem !important;
}

@media (max-width: 640px) {
 .carousel__prev {
    display: none;
  }

 .carousel__next {
    display: none;
  }
}
.circle-container {
 display: inline-block;
 position: relative;
}
.circle {
 position: relative;
 overflow: hidden;
}
.circle-fill {
 position: absolute;
 top: 0;
 left: 0;
}
.circle-progress {
 display: inline-block;
}
</style>


<script lang="ts" >
import { defineComponent } from 'vue'
import { Carousel, Pagination, Slide, Navigation } from 'vue3-carousel'
import 'vue3-carousel/dist/carousel.css'
export default defineComponent({
    name: 'MyCarousel',
    components: {
        Carousel,
        Slide,
        Pagination,
        Navigation,
    },
    data() {
        return {
            quotes: [
                'Per ricevere le nostre notizie via SMS e/o mesasaggi WhatsApp inserisci il numero di telefono',
                'Per ricevere le nostre notizie via SMS e/o mesasaggi WhatsApp inserisci il numero di telefono',
            ],
            activeSlide: 0,
            size: 190,
      percentage: 65,
      backgroundStrokeWidth: 4,
      foregroundStrokeWidth: 5
        };
    },
    methods: {
    updateActiveSlide(index){
      this.activeSlide = index;
    },

    updateSize() {
      const screenWidth = window.innerWidth;
      if (screenWidth<670) {
        this.size=150;
      }

      else{
       this.size=190;

      }
    },
  },
  mounted() {
    window.addEventListener('resize', this.updateSize);
    this.updateSize(); 

  },
  beforeUnmount() {
    window.removeEventListener('resize', this.updateSize);
  },
    computed: {
    radius() {
        return 50 - Math.max(this.backgroundStrokeWidth, this.foregroundStrokeWidth) / 2;
    },
    center() {
      return 50;
    },
    circumference() {
        return 2 * Math.PI * this.radius;
    },
    offset() {
        return this.circumference - (this.percentage / 100) * this.circumference;
    },
 },
})
</script> 