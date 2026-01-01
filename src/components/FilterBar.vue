<template>
  <div class="bg-white ">
    <div
      class="max-w-7xl mx-auto px-4 py-4
             flex flex-wrap items-center gap-3">

      <!-- SEARCH -->
      <div
        class="flex items-center border-2 border-[#0A5FD8]
               rounded-full h-11 px-4
               w-full md:w-105
               bg-[#F8FBFF]">

        <input
          class="flex-1 bg-transparent outline-none
                 text-sm text-gray-800"
          value="Austin, TX"
        />

        <!-- Clear -->
        <span
          class="text-gray-400 cursor-pointer px-2">
          ✕
        </span>

        <!-- Search Icon -->
        <button
          class="bg-[#0A5FD8] text-white h-8 w-8
                 rounded-full flex items-center justify-center">
          🔍
        </button>
      </div>

      <!-- ACTIVE FILTER -->
      <button
        class="h-11 px-5 rounded-lg text-sm font-medium
               border border-[#0A5FD8]
               bg-[#EAF2FF] text-[#0A5FD8]
               flex items-center gap-2">
        For Sale
        <span class="text-xs">▼</span>
      </button>

      <!-- NORMAL FILTERS -->
      <FilterButton label="Price" />
      <FilterButton label="Beds & Baths" />
      <FilterButton label="Property Type" />

      <!-- ICON FILTERS -->
      <FilterButton icon label="Filters" />
      <FilterButton icon label="Saved" />
    </div>
  </div>
</template>

<script setup>
import FilterButton from './FilterButton.vue'
</script>
