<template>
    <div class=" flex flex-col gap-4">
    <div class="conteiner  bg-[#F7F7F7]  p-8 rounded-3xl ">
        <div class="flex flex-row">
    <div class="w-1/4 flex flex-col">
    <h2 class="text-[#E72B6F] text-xl font-bold ">I tuoi dati</h2>
    <ul class="font-semibold space-y-4 my-6">
          <li>  Nome:
          <span class="font-normal"></span></li>
        <li>Cognome:<span class="font-normal"></span></li>
        <li>
            Data di nascita:<span class="font-normal"></span>
        </li>
        <li>Genere:<span class="font-normal"></span></li>
        <li>E-mail:<span class="font-normal"></span></li>
        <li>Cellulare:<span class="font-normal"></span></li>
        <li>Indirizzo:<span class="font-normal"></span></li>
        <li>CAP:<span class="font-normal"></span></li>
        <li>Provincia:<span class="font-normal"></span></li>
        <li>Data presunto parto:<span class="font-normal"></span></li>
    </ul>
    </div>
    <div class="w-1/4 translate-x-32  space-y-5 mx-12">
      <h2 class="text-[#E72B6F] text-xl font-bold">I tuoi consensi</h2>
      <p class="border-b-2 divide-y divide-[#DEDEDE] flex items-center justify-between">
        Puoi ricevere le nostre comunicazioni
        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5" class="w-6 h-6" stroke="green">
          <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
        </svg>
      </p>
      <p class="border-b-2 py-2 divide-y divide-[#DEDEDE] flex items-center justify-between">
        Puoi ricevere comunicazioni personalizzate
        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5" class="w-7 h-7" stroke="green">
          <path stroke-linecap="round" stroke-linejoin="round" d="m4.5 12.75 6 6 9-13.5" />
        </svg>
      </p>
      <p class="border-b-2 py-2 divide-y divide-[#DEDEDE] flex items-center justify-between">
        Puoi rispondere a survey e sondaggi
        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5" class="w-7 h-7" stroke="red">
          <path stroke-linecap="round" stroke-linejoin="round" d="M6 18 18 6M6 6l12 12" />
        </svg>
      </p>
      <p class="border-b-2 py-2 divide-y divide-[#DEDEDE] flex items-center justify-between">
        Puoi ricevere comunicazioni da altre società del Gruppo elo da soggetti Terzi
        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="3 0 24 24" stroke-width="3.5" class="w-16 h-16" stroke="red">
          <path stroke-linecap="round" stroke-linejoin="round" d="M6 18 18 6M6 6l12 12" />
        </svg>
      </p>
    </div>
    </div>
    <div class="flex flex-col">
        <!-- Title -->
        <h1 class="text-[#E72B6F] text-xl font-bold mb-4">La tua famiglia</h1>
        <div class="flex">
            <!-- First card -->
            <div class="flex items-center  bg-white border border-gray-200 rounded-lg shadow w-2/5 h-24 ">
                <img class="object-cover w-full rounded-t-lg h-44 md:h-auto md:w-16 md:rounded-none md:rounded-s-lg" src="assets\boyy.png" alt="">
                <div class="flex flex-col justify-between p-4 leading-normal">
                    <span class="mb-2 text-lg font-semibold tracking-tight text-[#E72B6F] dark:text-white">Name</span>
                    <p class=" font-medium tracking-tighter dark:text-gray-400">Data di nascita:</p>
                    <h6 class="font-medium tracking-tighter">Genere:</h6>
                </div>
            </div>
            <!-- Second card -->
            <div class="flex  translate-x-10 items-center bg-white border  rounded-lg shadow  w-2/5 h-24 ">
                <img class="object-cover w-full rounded-t-lg h-44 md:h-auto md:w-16 md:rounded-none md:rounded-s-lg" src="assets\girl.png" alt="">
                <div class="flex flex-col justify-between p-4 leading-normal">
                  <span class="mb-2 text-lg font-semibold tracking-tight text-[#E72B6F] dark:text-white">Name</span>
                    <p class=" font-medium tracking-tighter dark:text-gray-400">Data di nascita:</p>
                    <h6 class="font-medium tracking-tighter">Genere:</h6>
                </div>
            </div>
          </div>
        <!-- Third card -->
        <div class="flex flex-col mt-4">
            <div class="flex flex-row items-center bg-white border border-gray-200 rounded-lg shadow md:flex-row  w-2/5 h-24">
                <img class="object-cover w-full rounded-t-lg h-44 md:h-auto md:w-16 md:rounded-none md:rounded-s-lg" src="assets\girl.png" alt="">
                <div class="flex flex-col justify-between p-4 leading-normal">
                  <span class="mb-2 text-lg font-semibold tracking-tight text-[#E72B6F] dark:text-white">Name</span>
                    <p class=" font-medium tracking-tighter dark:text-gray-400">Data di nascita:</p>
                    <h6 class="font-medium tracking-tighter">Genere:</h6>
                </div>
            </div>
        </div>
        <a href="#" type="button" class="bg-[#E72B6F] translate-x-56 text-white py-3 px-5 w-40 rounded-full text-center font-medium mt-6">MODIFICA</a>
    </div>
        </div>
    <div class="flex flex-col  px-8 py-4 rounded-3xl border border-b-7 border-gray-300">
      <h2 class="text-[#E72B6F] text-lg font font-bold ">I tuoi badge</h2>
      <p>Completa le azioni per sbloccare più badge possibili!</p>
      <div class="flex flex-row space-x-6 translate-y-5">
    <!-- pregnant women -->
    <span class="rounded-full  bg-[#F9ECED] flex items-center justify-center">
        <div class="rounded-full h-16 w-16 bg-[#F9ECED] flex items-center justify-center">
            <svg fill="#E72B6F" height="50px" width="40px" version="1.2" baseProfile="tiny" id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="-217 51 256 256" xml:space="preserve">
                <path d="M-87.3,117.5c-17,0-30.9-13.7-30.9-30.7c0-16.9,13.8-30.6,30.9-30.6c17.1,0,30.9,13.7,30.9,30.6 C-56.4,103.8-70.2,117.5-87.3,117.5z"/>
                <path d="M5.3,244.5L-19,159.8c-9.7-33.9-38.1-32.8-38.1-32.8h-60.4c0,0-28.3-1.1-38.1,32.8l-24.3,84.7c-2.3,7.9,2,14,9,15.9 c6.9,2,14-1.5,15.8-7.8l23.6-82.6l11.6,0l-37.8,131.8h140.9L-54.7,170l11.5,0l23.7,82.6c1.8,6.3,8.9,9.8,15.8,7.8 C3.3,258.4,7.6,252.4,5.3,244.5z M-41.6,248.3c0,25.2-20.4,45.7-45.7,45.7c-25.2,0-45.7-20.5-45.7-45.7c0-25.2,20.4-45.7,45.7-45.7 C-62.1,202.6-41.6,223-41.6,248.3z"/>
                <path d="M-77.5,237.1c-5.5-2.6-7.8-9.1-5.2-14.6c2.6-5.5,9.1-7.8,14.6-5.2c5.5,2.6,7.8,9.1,5.2,14.6 C-65.5,237.4-72,239.7-77.5,237.1z"/>
                <path d="M-67.2,252.4c-1.1,2.3-6.9,14.5-8,16.9c-3.2,6.8-11.4,9.8-18.3,6.5c-2.2-1.1-3.9-2.7-5.4-4.5c-2.2-2.7-3.6-10-3.6-10 c-2.3,1.6-8.1,5.3-10.5,7c-2.2,1.5-5.2,1-6.8-1.2c-1.6-2.2-1-5.2,1.2-6.8c3.5-2.4,13.1-9,13.1-9c2.9-2.1,7-1.4,9,1.6l4.1,8.3 l6.5-13.1l-5.7-1.7c-1.2-0.4-2.3-1.2-2.9-2.4l-5.6-10.7c-1.2-2.3-0.3-5.2,2-6.4c2.3-1.2,5.2-0.3,6.4,2c0,0,3.3,6.4,4.6,8.9 c3.1,0.9,15.5,4.5,15.5,4.5c0.7,0.2,1.2,0.6,1.7,1C-66.9,245.4-65.7,249.2-67.2,252.4z"/>
            </svg>
        </div>
    </span>
    <span class="rounded-full  bg-[#F9ECED] flex items-center justify-center">
        <div class="rounded-full w-16 h-16 bg-[#F9ECED] flex items-center justify-center">
          <svg viewBox="0 0 24 24" fill="none" height="50px" width="40px"
     xmlns="http://www.w3.org/2000/svg"
    stroke="#E72B6F"><g id="SVGRepo_bgCarrier" stroke-width="0"></g>
    <g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round">
    </g><g id="SVGRepo_iconCarrier">
    <path d="M3 9H21M9 15L11 17L15 13M7 3V5M17 3V5M6.2 21H17.8C18.9201 21 19.4802 21 19.908 20.782C20.2843 20.5903 20.5903 20.2843 20.782 19.908C21 19.4802 21 18.9201 21 17.8V8.2C21 7.07989 21 6.51984 20.782 6.09202C20.5903 5.71569 20.2843 5.40973 19.908 5.21799C19.4802 5 18.9201 5 17.8 5H6.2C5.0799 5 4.51984 5 4.09202 5.21799C3.71569 5.40973 3.40973 5.71569 3.21799 6.09202C3 6.51984 3 7.07989 3 8.2V17.8C3 18.9201 3 19.4802 3.21799 19.908C3.40973 20.2843 3.71569 20.5903 4.09202 20.782C4.51984 21 5.07989 21 6.2 21Z"
    stroke="#E72B6F" stroke-width="1" stroke-linecap="round" stroke-linejoin="round"/></g></svg></div>
    </span>
    <!-- phone -->
    <span class="rounded-full  bg-[#F9ECED] flex items-center justify-center ">
        <div class="rounded-full w-16 h-16 bg-[#F9ECED] flex items-center justify-center">
          <svg viewBox="0 0 24 24" fill="none" width="50px" height="50px"
    xmlns="http://www.w3.org/2000/svg">
    <g id="SVGRepo_bgCarrier" stroke-width="1"></g>
    <g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g>
    <g id="SVGRepo_iconCarrier">
     <path d="M12 18.01V18M8 3H16C17.1046 3 18 3.89543 18 5V19C18 20.1046 17.1046 21 16 21H8C6.89543 21 6 20.1046 6 19V5C6 3.89543 6.89543 3 8 3Z"
    stroke="#E72B6F" stroke-width="1" stroke-linecap="round" stroke-linejoin="round"></path> </g></svg>
        </div>
    </span>
    <span class="rounded-full  bg-[#F9ECED] flex items-center justify-center">
        <div class="rounded-full w-16 h-16 bg-[#F9ECED] flex items-center justify-center">
            <svg fill="#E72B6F" width="30px" height="30px" viewBox="0 0 1920 1920" xmlns="http://www.w3.org/2000/svg">
                <path d="M0 1694.235h1920V226H0v1468.235ZM112.941 376.664V338.94H1807.06v37.723L960 1111.233l-847.059-734.57ZM1807.06 526.198v950.513l-351.134-438.89-88.32 70.475 378.353 472.998H174.042l378.353-472.998-88.32-70.475-351.134 438.89V526.198L960 1260.768l847.059-734.57Z"stroke-width="1"/>
            </svg>
        </div>
    </span>
    <span class="rounded-full  bg-[#F9ECED] flex items-center justify-center">
        <div class="rounded-full w-16 h-16 bg-[#F9ECED] flex items-center justify-center">
          <svg viewBox="0 0 24 24" width="50px" height="50px" fill="none" xmlns="http://www.w3.org/2000/svg"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g><g id="SVGRepo_iconCarrier"> <path d="M9 20H7C5.89543 20 5 19.1046 5 18V10.9199C5 10.336 5.25513 9.78132 5.69842 9.40136L10.6984 5.11564C11.4474 4.47366 12.5526 4.47366 13.3016 5.11564L18.3016 9.40136C18.7449 9.78132 19 10.336 19 10.9199V18C19 19.1046 18.1046 20 17 20H15M9 20V14C9 13.4477 9.44772 13 10 13H14C14.5523 13 15 13.4477 15 14V20M9 20H15" stroke="#E72B6F" stroke-linecap="round" stroke-linejoin="round"></path> </g>
          </svg></div>
          </span>
    <span class="rounded-full  bg-[#F9ECED] flex items-center justify-center">
        <div class="rounded-full w-16 h-16 bg-[#F9ECED] flex items-center justify-center">
          <svg class="h-8 w-8 text-[#E72B6F] "
          viewBox="0 0 24 24"  fill="none"  stroke="currentColor"
          stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round">
           <circle cx="9" cy="21" r="1" />  <circle cx="20" cy="21" r="1" />
             <path d="M1 1h4l2.68 13.39a2 2 0 0 0 2 1.61h9.72a2 2 0 0 0 2-1.61L23 6H6" /></svg>
        </div>
    </span>
    <span class="rounded-full  bg-[#F9ECED] flex items-center justify-center">
        <div class="rounded-full w-16 h-16 bg-[#F9ECED] flex items-center justify-center">
            <svg fill="#E72B6F" width="40" height="40" viewBox="0 0 24 24"  xmlns="http://www.w3.org/2000/svg">
                <circle cx="12" cy="10" r="7" fill="none" stroke="#E72B6F" stroke-width="2"/>
                <path d="M16.11 15.66 17 21 12 20 7 21 7.89 15.66" fill="none" stroke="#E72B6F" stroke-width="1" stroke-linecap="round" stroke-linejoin="round"/>
            </svg>
        </div>
    </span>
    </div>
    <a href="#" type="button" class="bg-[#E72B6F]  text-white py-3 -translate-x-14 w-40 mx-auto rounded-full text-center font-medium my-12">SCOPRI DI PIÙ</a>
    </div>
    </div>
    </template>