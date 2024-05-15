<template>
  <div class="">
    <div class="" v-if="!isMobile">
      <h1 class="text-4xl font-normal text-[#E72B6F]">Benvenuto/a</h1>
      <span class="text-4xl font-bold text-[#E72B6F]">Michela</span>
      <div class="flex flex-col lg:w-[270px] mt-10 table-border-collapse border-2 rounded-xl">
        <table>
          <tbody class="translate-x-9">
            <tr v-for="(tab, index) in tabs" :key="index" :class="{ 'rounded-t-lg': index === 0 }">
              <td
                class="px-2 py-3 font-normal text-xl "
                :class="{ 'border-t': index !== 0, 'border-b': index !== tabs.length - 1 }"
              >
                <router-link :to="tab.url" :class="{ 'text-[#E72B6F] font-semibold': isActiveTab(tab.url) }">{{ tab.name }}</router-link>
              </td>
            </tr>
          </tbody>
        </table>
      </div>
    </div>
    <div v-else>
      <div class="flex flex-row">
        <h1 class="text-2xl font-normal text-[#E72B6F]">Benvenuto/a</h1>
        <span class="text-2xl font-bold text-[#E72B6F]">Michela</span>
      </div>
      <button data-drawer-target="default-sidebar" @click="toggleDropdown" data-drawer-toggle="default-sidebar" aria-controls="default-sidebar" type="button" class="inline-flex items-center p-2 mt-2 ms-3 border-2 text-sm text-gray-500 rounded-lg sm:hidden hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-gray-200 dark:text-gray-400 dark:hover:bg-gray-700 dark:focus:ring-gray-600">
        <svg class="w-6 h-6" aria-hidden="true" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
          <path clip-rule="evenodd" fill-rule="evenodd" d="M2 4.75A.75.75 0 012.75 4h14.5a.75.75 0 010 1.5H2.75A.75.75 0 012 4.75zm0 10.5a.75.75 0 01.75-.75h7.5a.75.75 0 010 1.5h-7.5a.75.75 0 01-.75-.75zM2 10a.75.75 0 01.75-.75h14.5a.75.75 0 010 1.5H2.75A.75.75 0 012 10z"></path>
        </svg>
        <span class="">Open sidebar</span>
      </button>
      <div class="dropdown" v-if="isDropdownOpen">
        <div v-for="(tab, index) in tabs" :key="index">
          <router-link :to="tab.url" :class="{ 'text-[#E72B6F] font-semibold': isActiveTab(tab.url) }">{{ tab.name }}</router-link>
        </div>
      </div>
    </div>
  </div>
</template>
<script lang="ts">
import { defineComponent } from 'vue';
import { useRoute } from 'vue-router';
export default defineComponent({
  data() {
    return {
      tabs: [
        { name: 'La tua Card', url: '/user' },
        { name: 'I tuoi dati', url: '/tuoiDati' },
        { name: 'I tuoi Badge', url: '/badges' },
        { name: 'I tuoi Coupon', url: '/i-tuoi-coupon' },
        { name: 'Invita un amico', url: '/invitaUnAmico' },
        { name: 'Offerte esclusive', url: '/offerteEsclusive' },
        { name: 'Storico acquisti', url: '/storico-acquisti' },
        { name: 'FAQ', url: '/faq' },
        { name: 'Gestione ordini online', url: '/gestione-ordini-online' }
      ],
      isMobile: false,
      isDropdownOpen: false
    };
  },
  methods: {
    isActiveTab(url: string) {
      const route = useRoute();
      return route.path === url;
    },
    toggleDropdown() {
      this.isDropdownOpen = !this.isDropdownOpen;
    },
    checkIfMobile() {
      this.isMobile = window.innerWidth <= 900;
    }
  },
  mounted() {
    this.checkIfMobile();
    window.addEventListener('resize', this.checkIfMobile);
  },
  beforeDestroy() {
    window.removeEventListener('resize', this.checkIfMobile);
  }
});
</script>
<style scoped>
.dropdown {
  display: none;
}
@media screen and (max-width: 786px) {
  .w-1\4 {
    display: none;
  }
  .dropdown {
    display: block;
  }
}
</style>