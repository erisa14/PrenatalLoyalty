<template>
    <div>
      <h1 class="text-3xl font-normal text-[#E72B6F]">Benvenuto/a</h1>
      <span class="text-3xl font-bold text-[#E72B6F]">Michela</span>
      <div class="flex flex-col w-72 mt-6 table-border-collapse border-2  rounded-xl">
        <table>
          <tbody class=" translate-x-9">
            <tr v-for="(tab, index) in tabs" :key="index" :class="{ 'rounded-t-lg': index === 0 }">
              <td class="px-6 py-4 font-normal text-lg" :class="{ 'border-t': index !== 0, 'border-b': index !== tabs.length - 1 }">
                <a href="#" @click="activateTab(index)" :class="{ 'text-[#E72B6F] font-semibold': activeTab === index }">{{ tab }}</a>
              </td>
            </tr>
          </tbody>
        </table>
      </div>
    </div>
  </template>
  <script lang="ts">
  import { defineComponent } from 'vue';
  export default defineComponent({
    data() {
      return {
        activeTab: null as number | null,
        tabs: ['La tua Card', 'I tuoi dati', 'I tuoi Badge', 'I tuoi Coupon', 'Invita un amico', 'Offerte esclusive', 'Storico acquisti', 'FAQ', 'Gestione ordini online'] as string[]
      };
    },
    methods: {
      activateTab(index: number) {
        this.activeTab = index;
      }
    }
  });
  </script>
  <style scoped>
  .rounded-t-lg {
    border-top-left-radius: 20%;
    border-top-right-radius: 20%;
  }
  </style>