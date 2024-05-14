<!-- PinkOverlay.vue -->
<template>
    <div class="fixed inset-0 bg-pink-500 opacity-75" @click="closePinkPage">
        <ul
                    class="lg:flex flex-col font-medium p-4 lg:p-0 sm:space-x-5 lg:flex-row  w-full ">
                    <li>
                        <a href="#"
                            class="flex flex-row md:space-x-3 text-[#e82770] rounded font-semibold text-sm lg:text-lg pt-2"
                            aria-current="page">
                            <svg class="h-7 pt-1" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"
                                stroke-linecap="round" stroke-linejoin="round">
                                <circle cx="9" cy="21" r="1" />
                                <circle cx="20" cy="21" r="1" />
                                <path d="M1 1h4l2.68 13.39a2 2 0 0 0 2 1.61h9.72a2 2 0 0 0 2-1.61L23 6H6" />
                            </svg>
                            <span>Store online</span>
                        </a>
                    </li>
                    <li>
                        <button type="button"
                            class="bg-[#e82770] text-white hover:bg-pink-60 focus:ring-4 focus:outline-none focus:ring-pink-500 font-sans lg:text-lg text-sm font-normal px-5 py-2 logo text-center dark:bg-pink-600 dark:hover:bg-pink-700 dark:focus:ring-pink-800">ACCEDI
                            O REGISTRATI</button>
                    </li>
                </ul>
    </div>
  </template>
  
  <script>
  export default {
    methods: {
      closePinkPage() {
        this.$emit('close');
      },
    },
  };
  </script>
  