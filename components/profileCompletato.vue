<template>
    <div class="bg-[#f7f7f7] px-7 py-10 text-center rounded-2xl grid grid-col gap-10">
        <div>
            <h1 class="text-2xl font-semibold text-[#E72B6F] tracking-tight">Profilo Completato al</h1>
            <div id="app">
    <div class="circle-progress mt-8">
      <svg :width="size" :height="size" viewBox="0 0 100 100">
        <circle
          class="circle-progress__background"
          :r="radius"
          :cx="center"
          :cy="center"
          fill="none"
          stroke="#dddddd"
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
            <span>7 campi completati su 10</span>
        </div>
        <div>
            <h1 class="text-2xl font-semibold text-[#E72B6F] tracking-tight">Consigli</h1>
            <Carousel :autoplay="8000" :wrap-around="true" :items-to-show="1" @after-change="updateActiveSlide"
                v-model="activeSlide" class="mt-6">
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
        <a href="#" class="border border-[#E72B6F] rounded-3xl text-xl text-[#E72B6F] p-2 w-4/5 mx-auto mt-10">COMPLETA IL PROFILO</a>
    </div>
</template>
<script>
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

            size: 150,
      percentage: 65, 
      backgroundStrokeWidth: 6, 
      foregroundStrokeWidth: 7
        };
    },
    methods: {
        updateActiveSlide(index) {
            this.activeSlide = index;
        },
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

<style>
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