<template>
  <div>
    <nav>
      <Navbar></Navbar>
    </nav>


    <figure class="relative max-w-screen-2xl mx-auto md:top-10 ">

      <img class="rounded-3xl md:w-full md:h-auto h-[55vh]  w-[90%] mx-auto md:object-cover object-cover filter brightness-50 md:fill-none md:brightness-100" src="/assets/indexImage.jpg" alt="image description" style="object-position: 32% 50%;">
      <figcaption class="absolute self-center flex flex-col md:space-y-10 md:w-[40%] top-20 align-middle  justify-center text-white md:right-10">
        <h1 class="md:text-5xl text-4xl md:px-0 px-20 self-center md:self-start md:text-left text-center md:leading-12 leading-10 tracking-tight font-semibold  md:w-1/2">Entra nel club di Prénatal</h1>
        <p class="font-thin md:w-3/4 md:p-0 p-10 md:text-left  text-center  md:text-xl leading-tight ">Registrati gratuitamente per un mondo di promozioni dedicate,
          o acquista una VIP Card per accedere a tutti i vantaggi aggiuntivi.</p>
        <a href="#" class="md:px-3 md:py-2 md:w-2/5 w-[70%] rounded-3xl self-center md:self-start text-center text-white text-xl md:mb-0 mb-16 sm:mt-0 mt-4 py-3 bg-[#e82770]" type="button">ACCEDI
          O REGISTRATI</a>
        <h5 class="md:text-left text-center">Hai perso la tua card? <a href="#" class="underline">Recupera il codice</a></h5>
      </figcaption>

    </figure>

    <swiper
    :loop="true"
        :slides-per-view="2"
        :space-between="150"
        @slideChange="onSlideChange"
        @swiper="onSwiper"
        :pagination="true"
        :draggable="true"
    :autoplay="{
      delay: 1000,
    }"
    
     
  >
    <swiper-slide>   <div class="w-full max-w-sm rounded-xl text-center ">
          <h1 class="bg-[#e82770] text-2xl font-sans font-semibold text-white text-center p-7 rounded-t-3xl">Prénatal
            Card
          </h1>
          <div class="flow-root p-5 text-left shadow bg-[#ffedee] rounded-b-3xl">
            <ul class="divide-y divide-gray-50 text-lg tracking-wide font-sans font-semibold text-[#e82770]">
              <li></li>
              <li class="flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>
                Sarai informato in anteprima sulle promozioni
              </li>
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>Promozioni personalizzate per te
              </li>
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>Sconto di benvenuto
              </li>
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>Sconto speciale in occasione del compleanno di tuo figlio/a
              </li>
              <li class="flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>Offerte extra dai nostri brand partner
              </li>
              <li></li>
            </ul>
            <ul class="divide-y divide-gray-50 text-lg tracking-wide font-sans font-light" style="color: #909090;">
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M6 18 18 6M6 6l12 12" />
                  </svg></span>Sconti a partire dal -30%
              </li>
              <li class=" flex p-2 items-center ">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M6 18 18 6M6 6l12 12" />
                  </svg></span>
                Sconti a partire dal 30% su abbigliamento e arredo letto a marchio Prénatal
              </li>
              <li class=" flex p-2 items-center">
                <span>
                  <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M6 18 18 6M6 6l12 12" />
                  </svg></span>
                Sconti a partire dal 10% sui marchi Nike, Adidas, Nike Jordan, Vans, Converse, New Era e Puma
              </li>
              <li class=" flex px-3 py-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M6 18 18 6M6 6l12 12" />
                  </svg></span>Spedizione gratuita per ordini online*
              </li>
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M6 18 18 6M6 6l12 12" />
                  </svg></span>
                Servizio di personal shopper
              </li>

              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M6 18 18 6M6 6l12 12" />
                  </svg></span>
                Accesso all'esclusivo webinar di genitorialità
              </li>
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M6 18 18 6M6 6l12 12" />
                  </svg></span>
                Tantissimi vantaggi su una selezione di pannolini
              </li>
              <li></li>
            </ul>
            <h1 class="text-[#e82770] text-2xl font-sans font-bold text-center px-7 py-10 ">GRATIS</h1>


          </div>
          <div class="flex flex-col gap-7 px-16 -translate-y-1/4">
            <a href="#" class="button py-3 rounded-3xl top-10 text-white text-lg bg-[#e82770]">REGISTRATI SUBITO</a>
            <a href="#" class="underline text-gray-500 self-center font-thin">Regolamento Prénatal Card</a>
          </div>
        </div></swiper-slide>
    <swiper-slide>   <div class="w-full max-w-sm rounded-xl text-center ">
          <h1 class="bg-[#e82770] text-2xl font-sans font-semibold text-white text-center p-7 rounded-t-3xl">Prénatal
            Card
          </h1>
          <div class="flow-root p-5 text-left shadow bg-[#ffedee] rounded-b-3xl">
            <ul class="divide-y divide-gray-50 text-lg tracking-wide font-sans font-semibold text-[#e82770]">
              <li></li>
              <li class="flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>
                Sarai informato in anteprima sulle promozioni
              </li>
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>Promozioni personalizzate per te
              </li>
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>Sconto di benvenuto
              </li>
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>Sconto speciale in occasione del compleanno di tuo figlio/a
              </li>
              <li class="flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>Offerte extra dai nostri brand partner
              </li>
              <li></li>
            </ul>
            <ul class="divide-y divide-gray-50 text-lg tracking-wide font-sans font-light" style="color: #909090;">
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M6 18 18 6M6 6l12 12" />
                  </svg></span>Sconti a partire dal -30%
              </li>
              <li class=" flex p-2 items-center ">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M6 18 18 6M6 6l12 12" />
                  </svg></span>
                Sconti a partire dal 30% su abbigliamento e arredo letto a marchio Prénatal
              </li>
              <li class=" flex p-2 items-center">
                <span>
                  <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M6 18 18 6M6 6l12 12" />
                  </svg></span>
                Sconti a partire dal 10% sui marchi Nike, Adidas, Nike Jordan, Vans, Converse, New Era e Puma
              </li>
              <li class=" flex px-3 py-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M6 18 18 6M6 6l12 12" />
                  </svg></span>Spedizione gratuita per ordini online*
              </li>
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M6 18 18 6M6 6l12 12" />
                  </svg></span>
                Servizio di personal shopper
              </li>

              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M6 18 18 6M6 6l12 12" />
                  </svg></span>
                Accesso all'esclusivo webinar di genitorialità
              </li>
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M6 18 18 6M6 6l12 12" />
                  </svg></span>
                Tantissimi vantaggi su una selezione di pannolini
              </li>
              <li></li>
            </ul>
            <h1 class="text-[#e82770] text-2xl font-sans font-bold text-center px-7 py-10 ">GRATIS</h1>


          </div>
          <div class="flex flex-col gap-7 px-16 -translate-y-1/4">
            <a href="#" class="button py-3 rounded-3xl top-10 text-white text-lg bg-[#e82770]">REGISTRATI SUBITO</a>
            <a href="#" class="underline text-gray-500 self-center font-thin">Regolamento Prénatal Card</a>
          </div>
        </div></swiper-slide>
    <swiper-slide>Slide 3</swiper-slide>
    
  </swiper>

    <div class="sm:max-w-screen-2xl w-full mx-auto">
      <div class="flex sm:flex-row  flex-col justify-evenly sm:mt-12  sm:pt-20 sm:pb-10 px-5">
        <div class="max-w-sm bg-white p-5 flex flex-col justify-start mt-7 items-center">
          <div class="">
            <h1 class="mb-2 sm:text-4xl text-2xl w-2/3 sm:w-full font-semibold sm:font-bold tracking-tight text-[#e82770]" style="color: #e82770;">I vantaggi di
              entrare nel Club</h1>
            <p class="mb-3 font-normal font-serif leading-5 sm:leading-6 sm:text-lg">Registrati subito per vivere una esperienza di acquisto
              sempre
              piú personalizzata e in linea con le tue esigenze.</p>
          </div>
          <div class="sm:inline-block inline-flex gap-2 relative sm:top-24 sm:ml-20">
            <img class="rounded-xl sm:absolute drop-shadow-xl w-40 h-auto sm:w-[90%] sm:z-10 sm:rotate-12 sm:skew-y-6 top-24 sm:-translate-x-20"
              src="/assets/clubCard.png" alt="Prenatal vip club" />
            <img class="rounded-xl drop-shadow-xl w-40 h-auto sm:w-[90%] sm:-translate-y-3 sm:z-0 sm:-rotate-12  sm:-skew-y-6" src="/assets/pcard.png"
              alt="Prenatal card" />
            
          </div>
        </div>


        <div class="flex flex-row gap-8 justify-evenly">


        <div class="w-full max-w-sm rounded-xl text-center ">
          <h1 class="bg-[#e82770] text-2xl font-sans font-semibold text-white text-center p-7 rounded-t-3xl">Prénatal
            Card
          </h1>
          <div class="flow-root p-5 text-left shadow bg-[#ffedee] rounded-b-3xl">
            <ul class="divide-y divide-gray-50 text-lg tracking-wide font-sans font-semibold text-[#e82770]">
              <li></li>
              <li class="flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>
                Sarai informato in anteprima sulle promozioni
              </li>
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>Promozioni personalizzate per te
              </li>
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>Sconto di benvenuto
              </li>
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>Sconto speciale in occasione del compleanno di tuo figlio/a
              </li>
              <li class="flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>Offerte extra dai nostri brand partner
              </li>
              <li></li>
            </ul>
            <ul class="divide-y divide-gray-50 text-lg tracking-wide font-sans font-light" style="color: #909090;">
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M6 18 18 6M6 6l12 12" />
                  </svg></span>Sconti a partire dal -30%
              </li>
              <li class=" flex p-2 items-center ">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M6 18 18 6M6 6l12 12" />
                  </svg></span>
                Sconti a partire dal 30% su abbigliamento e arredo letto a marchio Prénatal
              </li>
              <li class=" flex p-2 items-center">
                <span>
                  <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M6 18 18 6M6 6l12 12" />
                  </svg></span>
                Sconti a partire dal 10% sui marchi Nike, Adidas, Nike Jordan, Vans, Converse, New Era e Puma
              </li>
              <li class=" flex px-3 py-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M6 18 18 6M6 6l12 12" />
                  </svg></span>Spedizione gratuita per ordini online*
              </li>
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M6 18 18 6M6 6l12 12" />
                  </svg></span>
                Servizio di personal shopper
              </li>

              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M6 18 18 6M6 6l12 12" />
                  </svg></span>
                Accesso all'esclusivo webinar di genitorialità
              </li>
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M6 18 18 6M6 6l12 12" />
                  </svg></span>
                Tantissimi vantaggi su una selezione di pannolini
              </li>
              <li></li>
            </ul>
            <h1 class="text-[#e82770] text-2xl font-sans font-bold text-center px-7 py-10 ">GRATIS</h1>


          </div>
          <div class="flex flex-col gap-7 px-16 -translate-y-1/4">
            <a href="#" class="button py-3 rounded-3xl top-10 text-white text-lg bg-[#e82770]">REGISTRATI SUBITO</a>
            <a href="#" class="underline text-gray-500 self-center font-thin">Regolamento Prénatal Card</a>
          </div>
        </div>

        <div class="w-full max-w-sm rounded-xl">
          <div
            class="flex flex-col justify-center text-center bg-[#dddddd] text-black rounded-full w-32 h-32 absolute rotate-12 translate-x-80 -translate-y-6">
            <h2 class="text-lg">risparmia</h2>
            <h1 class="text-[#3e5884] text-3xl font-bold">215€</h1>
            <h3 class="font-light text-xs ">in media <br>ogni anno*</h3>
          </div>
          <div class=" font-sans font-semibold text-white  px-7 py-4 rounded-t-3xl bg-[#3e5884]">
            <h1 class="text-2xl">Prénatal VIP Card</h1>
            <h5 class="text-[#cddfc5]">12 mesi di sconti esclusivi</h5>
          </div>
          <div class="flow-root p-5 text-left shadow text-[#e82770] bg-[#eaf1fd] rounded-b-3xl">
            <ul class="divide-y divide-gray-50 text-lg tracking-wide font-sans font-semibold">
              <li></li>
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>
                Sarai informato in anteprima sulle promozioni
              </li>
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>Promozioni personalizzate per te
              </li>
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>Sconto di benvenuto
              </li>
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>Sconto speciale in occasione del compleanno di tuo figlio/a
              </li>
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>Offerte extra dai nostri brand partner
              </li>
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>Sconti a partire dal -30%
              </li>
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>Sconti a partire dal 30% su abbigliamento e arredo letto a marchio Prénatal
              </li>
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>Sconti a partire dal 10% sui marchi Nike, Adidas, Nike Jordan, Vans, Converse, New Era e
                Puma
              </li>
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>Spedizione gratuita per ordini online*
              </li>
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>Servizio di personal shopper
              </li>

              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>Accesso all'esclusivo webinar di genitorialità
              </li>
              <li class=" flex p-2 items-center">
                <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5"
                    stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
                  </svg></span>Tantissimi vantaggi su una selezione di pannolini
              </li>
              <li></li>
            </ul>
            <div class="flex flex-col justify-between gap-3 py-5">
              <h1 class="text-[#e82770] text-2xl font-sans font-bold text-center  rounded-t-xl">30 €/anno</h1>
              <a href="#" class="text-center underline text-[#e82770] font-sans text-lg">Scopri tutti i vantaggi della
                VIP
                Card</a>
            </div>

          </div>
          <div class="flex flex-col gap-7 px-12 -translate-y-1/4">
            <a href="#" type="button"
              class="button py-3 rounded-3xl text-center text-white text-lg bg-[#e82770]">ACQUISTA
              LA TUA VIP CARD</a>
            <a href="#" class="underline text-gray-500 self-center font-thin">Regolamento VIP Card</a>
          </div>
        </div>
        </div>
      </div>
      <h5 class="text-right text-sm px-20 pb-5 font-semibold">*Sconto medio ottenuto dai clienti con VIP Card nel 2023
      </h5>

    </div>

    <VipReasones/>


    


    <figure class=" relative sm:max-w-screen-2xl mx-auto  grid  sm:mt-20">
      <img src="assets\p1.jpg" alt="image" class="sm:w-full sm:object-cover sm:object-left object-cover w-[90%] h-[75vh] mx-auto filter opacity-80  sm:h-[45%] rounded-3xl" style="object-position: 25% 50%;">
      <figcaption
        class="absolute sm:self-start self-end sm:py-0 py-10 sm:px-4 px-10 grid grid-col gap-5 text-lg font-normal font-serif sm:w-2/5 sm:top-20 sm:overflow-hidden  sm:right-60">
        <h1 class="sm:text-4xl text-2xl font-bold  text-[#e82770]">Parental Skills at Work</h1>
        <p class="sm:tracking-tight tracking-tighter sm:font-medium font-normal sm:text-xl text-[17px] leading-6 sm:leading-5">Se sei un cliente VIP, accedi gratuitamente al webinar
          legato alla genitorialità.
          Un percorso preparato per te con partners autorevoli per riscoprire come le skills genitoriali possono
          dare una marcia in più in famiglia e nella professione.</p>
        <a class="bg-[#e82770] font-xl sm:w-1/3 w-2/3 text-center px-5 py-3 rounded-full text-white">ACCEDI SUBITO
        </a>
      </figcaption>
      <div
        class="flex flex-col justify-center text-center -translate-x-12 -translate-y-16 bg-white rounded-full absolute w-48 h-48 text-sm">
        <span class="translate-x-20 translate-y-6 content-center"> <svg xmlns="http://www.w3.org/2000/svg"
            xmlns:xlink="http://www.w3.org/1999/xlink" width="57" height="48" viewBox="0 0 57 48">
            <defs>
              <pattern id="pattern" preserveAspectRatio="none" width="100%" height="100%" viewBox="0 0 82 70">
                <image width="82" height="70"
                  xlink:href="data:image/png;base64,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" />
              </pattern>
            </defs>
            <rect id="logo_parental_skills_at_work_compact" width="57" height="48" fill="url(#pattern)" />
          </svg></span>
        <h2 class="text-gray-600 text-lg  font-semibold translate-y-7 translate-x-4">parental</h2>
        <h3 class=" translate-y-6 font-light text-xs translate-x-4">skills at work</h3>
      </div>
    </figure>



    <happyBox class="sm:-mt-96 mt-10"/>

    <div class="sm:max-w-screen-2xl mx-auto max-w-screen-xl">

    <div class="relative sm:pt-8 sm:px-4 px-6">
      <h1 class=" text-[#E72B6F] sm:text-3xl text-2xl text-center sm:text-start font-bold ">Altri vantaggi esclusivi</h1>
      <div class="flex sm:flex-row flex-col justify-between sm:gap-0 gap-5 ">
        <p class="translate-y-4 text-lg from-neutral-700 text-center">Scopri le offerte attive in questo momento con i nostri
          partner selezionati, tutte riservate ai soli clienti registrati</p>
        <a href="#" type="button"
          class=" text-[#E72B6F] text-xl border-2 sm:text-right sm:right-24 text-center border-[#E72B6F] py-3 sm:px-5 rounded-full font-medium">SCOPRI
          DI PIÙ</a>
      </div>
    </div>

    <Carousel :autoplay="2000" :wrap-around="true" :items-to-show="itemsToShow"  @after-change="updateActiveSlide"
      v-model="activeSlide" class="responsive-screen mx-auto mt-10 mb-20">
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
      <p class="text-[#e82770] text-2xl font-bold mx-4">Hai giá una card?
        <a>
          <button class="bg-[#e82770] font-normal text-white text-xl mx-5 rounded-3xl px-5 py-3">ACCEDI</button>
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
import { Carousel, Pagination, Slide, Navigation } from 'vue3-carousel';
import { Swiper, SwiperSlide } from 'swiper/vue';

// Import Swiper styles
import 'swiper/swiper-bundle.css';

import 'vue3-carousel/dist/carousel.css';

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
      const onSwiper = (swiper) => {
        console.log(swiper);
      };
      const onSlideChange = () => {
        console.log('slide change');
      };
      return {
        onSwiper,
        onSlideChange,
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
    };
  },
  methods: {
    updateActiveSlide(index) {
      this.activeSlide = index;
    },
    updateItemsToShow() {
      const screenWidth = window.innerWidth;
      if (screenWidth <= 640) { 
        this.itemsToShow = 1.3; 
      } else {
        this.itemsToShow = 5; 
      }
    },
  },
  mounted() {
    window.addEventListener('resize', this.updateItemsToShow);
    this.updateItemsToShow(); 
  },
  beforeUnmount() {
    window.removeEventListener('resize', this.updateItemsToShow);
  },
});
</script>

<style>


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
