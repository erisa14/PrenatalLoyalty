<template>

    <nav>
        <Navbar />
    </nav>

    <div class="max-w-screen-2xl mx-auto flex mt-16">
        <LeftNav />

        <div class=" w-3/4 mx-auto mb-10 mt-16 flex flex-col gap-5">
            <figure class="relative -translate-y-16">

                <img class="rounded-3xl relative sm:w-full md:h-[600px] opacity-85" src="/assets/invita.png"
                    alt="image description">
                <figcaption class="absolute flex flex-col space-y-5 top-24 w-[46%] transform translate-x-[97%]">
                    <h1 class="text-[44px] leading-10 font-medium float-right text-[#e82770]">Invita un amico ad unirsi
                        al
                        nostro Fidelity Club</h1>
                    <p class="text-2xl leading-7 tracking-tight w-[90%]">Per ogni amico che sottoscrive la nostra Carta
                        Fedeltà per te uno sconto speciale di 10euro. Puoi farlo condividendo il link sottostante con
                        lui/lei.</p>


                    <div class="flex flex-row p-1">
                        <input type="text" :value="link" readonly
                            class=" border-2 border-r-0 px-8 py-3 rounded-l-md font-light text-lg w-full text-gray-500">
                        <button @click="copyLink" class="bg-[#e82770] p-3 rounded-r-md"><svg class="h-6 w-6 text-white"
                                width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor"
                                fill="none" stroke-linecap="round" stroke-linejoin="round">
                                <path stroke="none" d="M0 0h24v24H0z" />
                                <rect x="8" y="8" width="12" height="12" rx="2" />
                                <path d="M16 8v-2a2 2 0 0 0 -2 -2h-8a2 2 0 0 0 -2 2v8a2 2 0 0 0 2 2h2" />
                            </svg>
                        </button>
                    </div>

                    <div class="bg-[#e82770] text-white flex flex-row gap-2 w-1/3 rounded-3xl mt-8 py-1 px-6 ">
                        <svg class="w-10 h-10" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" width="32"
                            height="32" fill="none" viewBox="0 0 21 21">
                            <path stroke="white" stroke-linecap="round" stroke-width="2"
                                d="M7.926 10.898 15 7.727m-7.074 5.39L15 16.29M8 12a2.5 2.5 0 1 1-5 0 2.5 2.5 0 0 1 5 0Zm12 5.5a2.5 2.5 0 1 1-5 0 2.5 2.5 0 0 1 5 0Zm0-11a2.5 2.5 0 1 1-5 0 2.5 2.5 0 0 1 5 0Z" />
                        </svg>

                        <button @click="shareLink" class="w-35% text-xl mx-auto">CONDIVIDI</button>
                    </div>
                </figcaption>
            </figure>


            <div class="flex flex-col gap-7">
                <h1 class="text-4xl font-bold text-[#e82770]">Come funziona?</h1>
                <div class="flex gap-8">
                    <div class="bg-[#e82770] rounded-full sm:w-24 sm:h-24 flex justify-center items-center">
                        <svg width="92px" height="92px" viewBox="0 0 48 48" class="translate-x-2" fill="none"
                            xmlns="http://www.w3.org/2000/svg">
                            <g id="SVGRepo_bgCarrier" stroke-width="0"></g>
                            <g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g>
                            <g id="SVGRepo_iconCarrier">
                                <circle cx="24" cy="10" r="6" stroke="white" stroke-width="4" stroke-linecap="round"
                                    stroke-linejoin="round"></circle>
                                <path d="M28 44V36H38L27.2308 16H20.7692L10 36H20V44" stroke="white" stroke-width="4"
                                    stroke-linecap="round" stroke-linejoin="round"></path>
                            </g>
                        </svg>
                        <svg width="92px" height="92px" viewBox="0 0 48 48" class="-translate-x-1" fill="none"
                            xmlns="http://www.w3.org/2000/svg">
                            <g id="SVGRepo_bgCarrier" stroke-width="0"></g>
                            <g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g>
                            <g id="SVGRepo_iconCarrier">
                                <circle cx="24" cy="10" r="6" stroke="white" stroke-width="4" stroke-linecap="round"
                                    stroke-linejoin="round"></circle>
                                <path d="M28 44V36H38L27.2308 16H20.7692L10 36H20V44" stroke="white" stroke-width="4"
                                    stroke-linecap="round" stroke-linejoin="round"></path>
                            </g>
                        </svg>
                    </div>
                    <h3 class="sm:w-[90%] text-2xl">Invita un amico a sottoscrivere la nostra carta Fedeltà per entrare
                        in un mondo di vantaggi, promozioni speciali e sconti dedicati, validi in tutti i nostri negozi
                        e online</h3>
                </div>

                <div class="flex gap-8">

                    <div class="bg-[#e82770] rounded-full sm:w-24 sm:h-24 flex justify-center items-center">
                        <svg width="132px" height="62px" viewBox="-1 0 26 26" version="1.1"
                            xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"
                            xmlns:sketch="http://www.bohemiancoding.com/sketch/ns" fill="#000000">
                            <g id="SVGRepo_bgCarrier" stroke-width="0"></g>
                            <g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g>
                            <g id="SVGRepo_iconCarrier">
                                <title>share</title>
                                <defs> </defs>
                                <g id="Page-1" stroke="none" stroke-width="1" fill="none" fill-rule="evenodd"
                                    sketch:type="MSPage">
                                    <g id="Icon-Set" sketch:type="MSLayerGroup"
                                        transform="translate(-312.000000, -726.000000)" fill="white">
                                        <path
                                            d="M331,750 C329.343,750 328,748.657 328,747 C328,745.343 329.343,744 331,744 C332.657,744 334,745.343 334,747 C334,748.657 332.657,750 331,750 L331,750 Z M317,742 C315.343,742 314,740.657 314,739 C314,737.344 315.343,736 317,736 C318.657,736 320,737.344 320,739 C320,740.657 318.657,742 317,742 L317,742 Z M331,728 C332.657,728 334,729.343 334,731 C334,732.657 332.657,734 331,734 C329.343,734 328,732.657 328,731 C328,729.343 329.343,728 331,728 L331,728 Z M331,742 C329.23,742 327.685,742.925 326.796,744.312 L321.441,741.252 C321.787,740.572 322,739.814 322,739 C322,738.497 321.903,738.021 321.765,737.563 L327.336,734.38 C328.249,735.37 329.547,736 331,736 C333.762,736 336,733.762 336,731 C336,728.238 333.762,726 331,726 C328.238,726 326,728.238 326,731 C326,731.503 326.097,731.979 326.235,732.438 L320.664,735.62 C319.751,734.631 318.453,734 317,734 C314.238,734 312,736.238 312,739 C312,741.762 314.238,744 317,744 C318.14,744 319.179,743.604 320.02,742.962 L320,743 L326.055,746.46 C326.035,746.64 326,746.814 326,747 C326,749.762 328.238,752 331,752 C333.762,752 336,749.762 336,747 C336,744.238 333.762,742 331,742 L331,742 Z"
                                            id="share" sketch:type="MSShapeGroup"> </path>
                                    </g>
                                </g>
                            </g>
                        </svg>
                    </div>
                    <h3 class="sm:w-[90%] text-2xl">Condividi il tuo link personale con chi vuoi. Puoi mandarlo via
                        Whatsapp, Facebook o via email, come preferisci!</h3>
                </div>
                <div class="flex gap-8">
                    <div class="bg-[#e82770] rounded-full sm:w-24 sm:h-24 flex justify-center items-center">
                        <svg xmlns="http://www.w3.org/2000/svg" width="50" height="50" class="" viewBox="0 0 16 16">
                            <path fill="white" fill-rule="evenodd"
                                d="M6.427.512A1.75 1.75 0 0 1 7.664 0H13v3h3v5.335c0 .465-.185.91-.513 1.239L9.573 15.48a1.75 1.75 0 0 1-2.473 0l-2.293-2.293l-1.293-1.293l-3-3a1.75 1.75 0 0 1 0-2.475L6.428.512ZM11.5 1.5V3h-.836a1.75 1.75 0 0 0-1.237.512L3.514 9.419q-.09.09-.165.19L1.574 7.833a.25.25 0 0 1 0-.353l5.913-5.907a.25.25 0 0 1 .177-.073zM5.866 12.126l-1.292-1.293a.25.25 0 0 1 0-.353l5.913-5.907a.25.25 0 0 1 .177-.073H14.5v3.835a.25.25 0 0 1-.073.177L8.513 14.42a.25.25 0 0 1-.353 0zM12 8a1 1 0 1 0 0-2a1 1 0 0 0 0 2"
                                clip-rule="evenodd" />
                        </svg>
                    </div>
                    <h3 class="sm:w-[90%] text-2xl">Quando il tuo amico avrà terminato la registrazione utilizzando il
                        tuo link, entrambi riceverete uno sconto subito valido per il vostro prossimo acquisto: per te
                        uno sconto di 10€, per il tuo amico uno sconto di 15€!</h3>
                </div>


            </div>

            <div class="bg-[#f7f7f7] flex flex-col gap-5 p-12 rounded-3xl mt-16">
                <h1 class="text-[#e82770] text-3xl font-medium">I tuoi inviti</h1>
                <div class="flex">
                    <p class="bg-[#e82770] rounded-l-xl p-5">
                        <svg width="72px" height="72px" viewBox="0 0 48 48" fill="none"
                            xmlns="http://www.w3.org/2000/svg">
                            <g id="SVGRepo_bgCarrier" stroke-width="0"></g>
                            <g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g>
                            <g id="SVGRepo_iconCarrier">
                                <circle cx="24" cy="10" r="6" stroke="white" stroke-width="4" stroke-linecap="round"
                                    stroke-linejoin="round"></circle>
                                <path d="M31 44V35L36 32L32 19C32 19 28 16 24 16C20 16 16 19 16 19L12 31L17 35V44"
                                    stroke="white" stroke-width="4" stroke-linecap="round" stroke-linejoin="round">
                                </path>
                            </g>
                        </svg>
                    </p>
                    <div class="flex flex-row justify-between w-full px-8 bg-white items-center text-[#e82770]">
                        <h2 class=" text-3xl font-bold">Michele</h2>
                        <h3 class="text-xl font-medium sm:w-[28%] border-l-2 border-gray-200 pl-3">Registrazione
                            effettuata</h3>
                    </div>

                </div>
                <div class="flex">
                    <p class="bg-[#e82770] rounded-l-xl p-5">

                        <svg width="72px" height="72px" viewBox="0 0 48 48" fill="none"
                            xmlns="http://www.w3.org/2000/svg">
                            <g id="SVGRepo_bgCarrier" stroke-width="0"></g>
                            <g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g>
                            <g id="SVGRepo_iconCarrier">
                                <circle cx="24" cy="10" r="6" stroke="white" stroke-width="4" stroke-linecap="round"
                                    stroke-linejoin="round"></circle>
                                <path d="M28 44V36H38L27.2308 16H20.7692L10 36H20V44" stroke="white" stroke-width="4"
                                    stroke-linecap="round" stroke-linejoin="round"></path>
                            </g>
                        </svg>
                    </p>
                    <div class="flex flex-row justify-between w-full px-8 bg-white items-center text-[#e82770]">
                        <h2 class=" text-3xl font-bold">Marzia</h2>
                        <h3 class="text-xl font-medium sm:w-[28%] border-l-2 border-gray-200 pl-3">Richiesta inviata
                        </h3>
                    </div>

                </div>
            </div>
        </div>
    </div>

    <Footer></Footer>
</template>


<script>

export default defineComponent({
    name: 'LinkComponent',
    name: 'ShareButtonComponent',


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
        };
    },
    data() {
    },
    methods: {


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
