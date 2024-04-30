<template>
    <nav>
        <Navbar />
    </nav>

    <div class="max-w-screen-2xl mx-auto flex mt-16">
        <LeftNav />

        <div class=" w-3/4 mx-auto mb-10 mt-16">
        <figure class="relative -translate-y-16">

            <img class="rounded-3xl relative w-full h-[90%] opacity-85" src="/assets/invita.png"
                alt="image description">
            <figcaption class="absolute flex flex-col space-y-5 top-24 w-[46%] transform translate-x-[97%]">
                <h1 class="text-[44px] leading-10 font-medium float-right text-[#e82770]">Invita un amico ad unirsi al
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

                <div class="bg-[#e82770] text-white flex flex-row gap-2 w-1/3 rounded-3xl mt-8 py-3 px-6 ">
                    <svg class="w-10 h-10" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" width="32" height="32" fill="none" viewBox="0 0 21 21">
  <path stroke="white" stroke-linecap="round" stroke-width="2" d="M7.926 10.898 15 7.727m-7.074 5.39L15 16.29M8 12a2.5 2.5 0 1 1-5 0 2.5 2.5 0 0 1 5 0Zm12 5.5a2.5 2.5 0 1 1-5 0 2.5 2.5 0 0 1 5 0Zm0-11a2.5 2.5 0 1 1-5 0 2.5 2.5 0 0 1 5 0Z"/>
</svg>

                    <button @click="shareLink" class="w-35% text-xl mx-auto">CONDIVIDI</button>
                </div>
            </figcaption>
        </figure>


        <div><h1>Come funziona?</h1>
            <svg class="w-6 h-6 text-gray-800 dark:text-white" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" viewBox="0 0 24 24">
  <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15.583 8.445h.01M10.86 19.71l-6.573-6.63a.993.993 0 0 1 0-1.4l7.329-7.394A.98.98 0 0 1 12.31 4l5.734.007A1.968 1.968 0 0 1 20 5.983v5.5a.992.992 0 0 1-.316.727l-7.44 7.5a.974.974 0 0 1-1.384.001Z"/>
</svg>
<svg class="w-6 h-6 text-gray-800 dark:text-white" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" viewBox="0 0 24 24">
  <path stroke="currentColor" stroke-linecap="round" stroke-width="2" d="M7.926 10.898 15 7.727m-7.074 5.39L15 16.29M8 12a2.5 2.5 0 1 1-5 0 2.5 2.5 0 0 1 5 0Zm12 5.5a2.5 2.5 0 1 1-5 0 2.5 2.5 0 0 1 5 0Zm0-11a2.5 2.5 0 1 1-5 0 2.5 2.5 0 0 1 5 0Z"/>
</svg>


                    
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
