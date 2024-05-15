
<template>
  <Navbar/>
  <div :class="{ 'shadow-gray': showAlert }" class="max-w-screen-xl mx-auto flex flex-col mt-16">
      <div class="md:flex flex-row gap-12 mx-auto">
      <div class="w-1/4">
          <LeftNav/>
      </div>
      <div class="w-full flex flex-col px-6">
      <div class="flex flex-row  justify-end text-lg "> <span><svg class="w-4 h-8 solosvg text-gray-600 dark:text-white" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" width="4" height="8" fill="none" viewBox="0 0 24 24">
        <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="3" d="m15 19-7-7 7-7"/>
      </svg>
      </span><a href="/page4" class="text-[#E72B6F] solosvg ">Torna alla pagina principale</a>
      </div>
      <div class="md:flex flex-col h-1/4">
          <img src="/assets/yoga.jpg" alt="yogare image" class="md:w-auto md:h-full w-full h-32 mt-4 rounded-lg">
          <img src="https://storage.googleapis.com/prg-loyalty.appspot.com/media/102/img-logo---595x422px.jpg
" alt="yogare logo"class="md:-translate-y-32  -translate-y-14 mx-auto md:w-5/12 md:h-60 w-[60%] h-32 self-center rounded-2xl" >
      </div>
      <a href="#" type="button" class="w-52 h-10 text-center bg-[#3E5884] p-2 solosvg text-white font-medium mt-20 rounded-3xl "> SOLO CON VIP CARD</a>
      <div class="md:py-6 p-2 space-y-4">
          <h1 class="text-[#E72B6F] md:text-4xl text-3xl font-semibold  md:font-medium ">Sconto di 50% sull'abbonamento mensile con Yogare.</h1>
          <h4 class="md:text-3xl text-xl font-light tracking-tight ">Scade il: 30/04/2024</h4>
          <p class="md:text-2xl text-lg  md:tracking-normal tracking-tighter font-normal text-wrap py-8 ">Vuoi trovare il tuo benessere in modo naturale con lo yoga? Per te che sei cliente Toys Center, Bimbostore & FAO Schwarz attiva subito il tuo abbonamento scontato del 50% a Yogare per tuffarti nel primo studio di yoga online dove, con insegnanti esperti, puoi praticare tecniche di movimento, meditazione, espansione del respiro e di rilassamento profondo. Hai a disposizione oltre 600 lezioni, 7 giorni su 7, 24 ore su 24.</p>
      </div>
      <button @click="showAlert = true" class="md:mt-8 bg-[#E82770] text-white md:text-xl rounded-full w-60 h-14 p-3 text-center">RICHIEDI CODICE</button>
      <div class="my-20 font-normal text-2xl space-y-4">
          <h5 class="text-[#E72B6F] font-semibold ">Utilizzo:</h5>
          <ul class="pink-bullets md:text-2xl text-xl tracking-tighter ">
              <li>Vai sul sito https://yogare.eu/partner/</li>
              <li>Seleziona il vantaggio che sarà aggiunto al carrello</li>
              <li>Inserisci il codice sconto e termina l'acquisto</li>
              <li >Validità dell'offerta: dal 01/01/2024 al 30/04/2024 con validità codici fino al 31/05/2024</li>
          </ul>
      </div>
      <div class="md:text-2xl text-xl tracking-tighter">
          <h4 class="text-[#E72B6F] text-2xl font-semibold">Termini e condizioni:</h4>
          <p class=" mt-6">L'offerta è valida sia per nuovi clienti sia per vecchi clienti inattivi che hanno già utilizzato un periodo di free trial. Il codice sconto si applica al carrello, è utilizzabile una sola volta, non è cumulabile con altri codici sconto e/o altre promo attive sul sito. Non è previsto un meccanismo di alert che informa il cliente della scadenza del mese scontato e del rinnovo.</p>
          <p class=" md:my-6  mt-6 mb-32 ">Per assistenza e informazioni: help@yogare.eu</p>
      </div>
      <div class="">
          <div v-if="showAlert" class="alert">
            <button class="close-btn md:right-8 right-20" @click="closeAlert">
              <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" version="1.1" width="14" height="16" viewBox="0 0 256 256" xml:space="preserve">
      <defs>
      </defs>
      <g style="stroke: none; stroke-width: 0; stroke-dasharray: none; stroke-linecap: butt; stroke-linejoin: miter; stroke-miterlimit: 1; fill: none; fill-rule: nonzero; opacity: 1;" transform="translate(1.4065934065934016 1.4065934065934016) scale(2.81 2.81)" >
          <path d="M 6 90 c -1.536 0 -3.071 -0.586 -4.243 -1.758 c -2.343 -2.343 -2.343 -6.142 0 -8.484 l 78 -78 c 2.342 -2.343 6.143 -2.343 8.484 0 c 2.344 2.343 2.344 6.142 0 8.485 l -78 78 C 9.071 89.414 7.536 90 6 90 z" style="stroke: none; stroke-width: 1; stroke-dasharray: none; stroke-linecap: butt; stroke-linejoin: miter; stroke-miterlimit: 10; fill: rgb(0,0,0); fill-rule: nonzero; opacity: 1;" transform=" matrix(1 0 0 1 0 0) " stroke-linecap="round" />
          <path d="M 84 90 c -1.535 0 -3.071 -0.586 -4.242 -1.758 l -78 -78 c -2.343 -2.343 -2.343 -6.142 0 -8.485 c 2.343 -2.343 6.143 -2.343 8.485 0 l 78 78 c 2.344 2.343 2.344 6.142 0 8.484 C 87.071 89.414 85.535 90 84 90 z" style="stroke: none; stroke-width: 1; stroke-dasharray: none; stroke-linecap: butt; stroke-linejoin: miter; stroke-miterlimit: 10; fill: rgb(0,0,0); fill-rule: nonzero; opacity: 1;" transform=" matrix(1 0 0 1 0 0) " stroke-linecap="round" />
      </g>
      </svg>
          </button>
          <div class="flex items-center p-9">
              <div class="rounded-full md:w-80 w-44 h-24 md:h-32 bg-[#F7F7F7]">
                <img src="assets/clubCard.png" alt="Photo" class="md:w-28 w-28 h-auto rounded-xl -rotate-12 md:mt-7 mt-4 md:mx-4 px-2 p-2">
              </div>
              <h1 class="ml-6 text-[#435D87] font-semibold md:text-3xl text-xl ">{{ alertText }}</h1>
            </div>
            <button class="btn m-8 rounded-3xl text-xl" @click="submit">ACQUISTA VIP CARD</button>
          </div>
      </div>
      <div v-if="showAlert" class="overlay"></div>
      </div>
      </div>
      <div>
      </div></div>
      <Footer></Footer>
      </template>
      <style scoped>
      .pink-bullets li::before {
              content: "•";
              color: #F2D5D6;
              display: inline-block;
              width: 1em;
              font-size: 1.9em;
              margin-left: 0em;
          }
      .alert {
        position: fixed;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        background-color: #fff;
        border: 1px solid #ccc;
        border-radius: 20px;
        padding: 20px;
        box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
        max-width: 650px;
        width: 110vw;
        max-height: 350px;
        height: 100vw;
        z-index: 999;
      }
      .close-btn {
        position: absolute;
        background-color: transparent;
        border: none;
        cursor: pointer;
        font-size: 2rem;
      }
      .btn {
        padding: 12px 16px;
        background-color: #E72B6F;
        color: #fff;
        border: none;
        cursor: pointer;
        max-width: 550px;
        width: 80vw;
      }
      .overlay {
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background-color: rgba(0, 0, 0, 0.5);
        z-index: 998;
      }
      .shadow-gray {
        box-shadow: 0px 0px 20px rgba(0, 0, 0, 0.1);
      }
      @media screen and (max-width: 786px) {
        .solosvg{
            display: none;
         }
      }
      </style>

<script>
export default {
  data() {
    return {
      showAlert: false,
      alertText: 'Questa offerta è riservata esclusivamente ai clienti con VIP Card.'
    };
  },
  methods: {
    submit() {
      this.showAlert = true;
    },
    closeAlert() {
      this.showAlert = false;
    }
  }
};
</script>