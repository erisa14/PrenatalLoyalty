<template>
    <Navbar />
    <div class=" lg:w-[65%] md:w-[80%] w-[92%] mx-auto flex flex-col mt-16">
        <LeftNav class=" lg:hidden block " />
        <div class="flex lg:flex-row lg:gap-5 flex-col">
            <div class=" lg:block hidden">
                <LeftNav />
            </div>
            <div class="flex flex-col lg:gap-6 gap-3 lg:w-[51%] md:w-[80%] w-[92%] mx-auto lg:mt-0 mt-5">
                <div class="bg-[#EAF1FD] px-6 pt-1 pb-12 rounded-3xl">
                    <h1 class="text-[#E73B7A]  md:text-xl text-2xl font-bold tracking-tighter py-5">La tua Fidelity Card</h1>
                    <div class=" flex md:flex-row flex-col gap-6">
                        <div class="">
                            <img src="assets\vip_card.png" class="rounded-3xl w-auto lg:h-52 md:h-40 h-52" alt="Prenatal Card">
                            <h2 class="-translate-y-10 text-center font-semibold md:text-lg text-sm tracking-wider">{{ cardNumber
                                }}</h2>
                        </div>
                        <div class="flex flex-col gap-2 md:w-1/3 ">
                            <h2 class="text-[#E73B7A] md:text-base text-lg tracking-tighter font-semibold leading-3">Numero Card: <span class="text-black mx-4 text-lg">{{ cardNumber }}</span></h2>
                            <p class="font-semibold text-lg tracking-tight md:block hidden">{{ cardNumber }}</p>
                            <div class="flex flex-row gap-2 text-lg tracking-tighter">
                                <h2 class="text-[#E73B7A] font-semibold">Stato:</h2>
                                <h3>Attiva</h3>
                            </div>
                            <div class="flex text-lg gap-4 tracking-tighter font-semibold text-[#FE720C]">
                                <h2 class="text-[#E73B7A]">Scadenza: </h2>
                                <h3>29/05/2024</h3>
                            </div>
                            <div class="flex text-md gap-1 tracking-tighter font-semibold text-[#FE720C]">
                                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24"
                                    stroke-width="2.5" stroke="currentColor" class="w-6 h-6 md:translate-y-1 -translate-y-1">
                                    <path stroke-linecap="round" stroke-linejoin="round"
                                        d="M12 9v3.75m9-.75a9 9 0 1 1-18 0 9 9 0 0 1 18 0Zm-9 3.75h.008v.008H12v-.008Z" />
                                </svg>
                                <h4 class="tracking-tighter leading-4 text-sm lg:w-3/4">La tua card sta per scadere,
                                    rinnova subito!</h4>
                            </div>
                            <a href="#"><button class="bg-[#E82770] rounded-3xl text-white lg:py-3 lg:mt-6 lg:px-6 md:px-3 md:py-2 w-full py-3">RINNOVA LA
                                    CARD</button></a>
                        </div>
                    </div>
                </div>
                <div>
                    <Dati class="hidden lg:flex " />
                </div>
            </div>
            <div class="grid grid-col  lg:gap-6 md:gap-6 gap-6">
                <article
                    class="relative isolate flex flex-col lg:justify-end rounded-2xl lg:px-8 lg:gap-0 md:gap-4 lg:pb-6 lg:pt-24 lg:w-full md:w-[80%] w-[92%] md:pt-72 pt-60 mx-auto">
                    <img src="/assets/p-skills.png" alt="Parental Skills"
                        class="absolute  inset-0 w-full lg:h-[37vh] h-auto ">
                    <h3 class="z-10 lg:mt-10 lg:text-[22px] text-3xl font-bold text-[#E82770] text-center ">Parental Skills at Work
                    </h3>
                    <p class="z-10 lg:text-lg md:text-2xl font-normal tracking-tighter lg:leading-5 lg:w-full w-2/3 mx-auto  text-center mb-5">Accedi
                        gratuitamente al
                        webinar legato alla genitorialità. Riscopri tue skills genitoriali con i nostri autorevoli
                        partners.</p>
                    <button class="z-10 bg-[#E82770] text-white lg:text-lg text-xl rounded-3xl py-3 lg:px-7 px-10 mx-auto lg:mb-0 md:mb-16 mb-12 ">ACCEDI
                        GRATIS</button>
                </article>

                <profileCompletato class=" lg:w-full md:w-[80%] w-[92%] mx-auto lg:mt-10"/>
        <Dati class="lg:hidden flex"/>
        <div class="grid grid-col px-9 pt-4 rounded-3xl border border-gray-300 gap-6 lg:w-full md:w-[80%] w-[92%] mx-auto">
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
        <Vantaggi class="lg:ml-72 mx-auto" />
        <HappyBox />
    </div>
    <Footer></Footer>
</template>
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