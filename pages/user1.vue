<template>
    <Navbar />
    <div class="max-w-screen-2xl mx-auto flex flex-col mt-16">
        <div class="flex flex-row gap-7 mx-auto ">
        <div>
          <LeftNav/>
        </div>
      <div class="flex flex-col gap-4 w-2/4">
                <div class="bg-[#f9eced] px-6 pt-5 pb-16 rounded-3xl">
                    <h1 class="text-[#e73b7a] text-xl font-bold tracking-tighter py-5">La tua Fidelity Card</h1>
                    <div class=" flex flex-row gap-6">
                        <div class="">
                            <img src="/assets/vip_card.png" class="rounded-xl" alt="Prenatal Card">
                            <h2 class="-translate-y-10 text-center font-semibold text-xl tracking-wider">{{ cardNumber }}</h2>
                        </div>
                        <div class="flex flex-col gap-1 w-1/2">
                            <h2 class="text-[#e73b7a] text-lg tracking-tighter font-semibold">Numero Card:</h2>
                            <p class=" font-semibold text-xl tracking-wider">{{ cardNumber }}</p>
                            <div class="flex flex-row gap-2 text-lg tracking-tighter">
                                <h2 class="text-[#e73b7a] font-semibold">Stato:</h2>
                                <h3>Attiva</h3>
                            </div>
                            <div class="flex text-lg gap-4 tracking-tighter font-semibold text-[#fe720c]">
                                <h2 class="text-[#e73b7a]">Scadenza: </h2>
                                <h3>29/05/2024</h3>
                            </div>
                            <div class="flex text-md gap-2 tracking-tighter font-semibold text-[#fe720c]"><svg
                                    xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24"
                                    stroke-width="2.5" stroke="currentColor" class="w-8 h-8 translate-y-2">
                                    <path stroke-linecap="round" stroke-linejoin="round"
                                        d="M12 9v3.75m9-.75a9 9 0 1 1-18 0 9 9 0 0 1 18 0Zm-9 3.75h.008v.008H12v-.008Z" />
                                </svg>
                                <h4 class="w-3/4">La tua card sta per scadere rinnovala subito!</h4>
                            </div>
                            <a href="#"><button
                                    class="bg-[#E82770] rounded-3xl text-white py-3 mt-6 px-6 text-lg">RINNOVA LA
                                    CARD</button></a>
                        </div>
                    </div>

                </div>
                <Dati/>

            </div>

            <div class="grid grid-col gap-3 w-1/4">
                <article class="relative isolate flex flex-col justify-end overflow-hidden rounded-2xl px-8 pb-8 pt-40">
                    <img src="/assets/parental_skills.png" alt="Parental Skills"
                        class="absolute inset-0 w-full object-cover">
                    <div class="svg-container absolute top-0 left-0">
                        <svg width="100" height="100" view-box="0 0 100 100">
                            <circle cx="28" cy="25" r="51" fill="white" />
                            
                            <text x="15" y="45" font-size="9px" letter-spacing="1"  fill="gray">parental</text>
                            <text x="15" y="52" font-size="6px" letter-spacing="0.5" fill="gray">skills at work</text>

            <defs>
              <pattern id="pattern" width="100%" height="100%" viewBox="0 0 70 70">
                <image  height="50" x="-20" y="8"
                  xlink:href="data:image/png;base64,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" />
              </pattern>
            </defs>
            <rect id="logo_parental_skills_at_work_compact" width="100%" height="40" fill="url(#pattern)" />
         
                        </svg>
                    </div>
                    <div class="absolute inset-0"></div>
                    <h3 class="z-10 mt-3 text-2xl font-bold text-[#e82770] text-center mb-3">Parental Skills at Work
                    </h3>
                    <div class="z-10 text-md font-normal tracking-tight leading-5 px-12 text-center mb-5">Accedi gratuitamente al
                        webinar legato alla genitorialità. Riscopri tue skills genitoriali con i nostri autorevoli
                        partners.</div>
                    <button class="z-10 bg-[#e82770] text-white text-xl rounded-3xl py-3 w-2/3 self-center">ACCEDI
                        GRATIS</button>
                </article>

                <profileCompletato />
                <div class="grid grid-col gap-5 px-9 py-10 rounded-3xl border border-gray-300">
                    <h1 class="text-[#e82770] text-2xl font-semibold">Invita un amico</h1>
                    <div>
                        <p class="text-lg tracking-tight leading-5 ">Condividi i link con un tuo amico e ricevi uno
                            sconto di 10 euro.
                        </p>
                        <a href="#" class="underline leading-3">Scopri di piú</a>
                    </div>
                    <div class="flex flex-row">
                        <input type="text" :value="link" readonly
                            class="border border-1 px-8 py-3 rounded-l-md font-light text-lg text-gray-300">
                        <button @click="copyLink" class="bg-[#e82770] p-3 rounded-r-md"><svg class="h-6 w-6 text-white"
                                width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor"
                                fill="none" stroke-linecap="round" stroke-linejoin="round">
                                <path stroke="none" d="M0 0h24v24H0z" />
                                <rect x="8" y="8" width="12" height="12" rx="2" />
                                <path d="M16 8v-2a2 2 0 0 0 -2 -2h-8a2 2 0 0 0 -2 2v8a2 2 0 0 0 2 2h2" />
                            </svg>
                        </button>
                    </div>

                    <div class="bg-[#e82770] text-white flex flex-row gap-2 rounded-3xl mt-8 py-3 px-6 w-35% mx-auto">
                        <svg class="h-6 w-6 mx-auto" viewBox="0 0 24 24" fill="none" stroke="currentColor"
                            stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                            <circle cx="18" cy="5" r="3" />
                            <circle cx="6" cy="12" r="3" />
                            <circle cx="18" cy="19" r="3" />
                            <line x1="8.59" y1="13.51" x2="15.42" y2="17.49" />
                            <line x1="15.41" y1="6.51" x2="8.59" y2="10.49" />
                        </svg>
                        <button @click="shareLink" class="  text-xl mx-auto">CONDIVIDI</button>
                    </div>

                </div>
            </div>
        </div>
        <Vantaggi class="ml-auto" />
        <HappyBox />
    </div>
    <Footer></Footer>

</template>


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

<style>
.carousel-content {
    font-size: 16px;
    color: black;
    width: 75%;
    height: max-content;
    padding: 10%;
    border: 2px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    transition: box-shadow 0.3s ease-out;
    padding-top: 12%;
    padding-bottom: 12%;
    border-radius: 0.5rem !important;
}

.active-quote {
    transform: scale(1);
    z-index: 1;
    height: auto;
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
    background-color: #2c5c89;
}

.carousel__icon:hover {
    color: #e82770;
}

.carousel__icon.isActive {
    color: #e82770;
}

</style>