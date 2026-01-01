<script setup>
defineProps({
  image: String,
  typeLabel: String
})
</script>

<template>
  <div class="bg-white rounded-2xl border border-gray-200 hover:shadow-lg transition overflow-hidden">

    <!-- IMAGE -->
    <div class="relative h-45 bg-gray-200">
      <img
        :src="image"
        class="absolute inset-0 w-full h-full object-cover"
        alt="Property"
      />

      <span class="absolute top-3 left-3 bg-white text-xs px-3 py-1 rounded-full shadow">
        6 days on Houzeo
      </span>

      <button
        class="absolute top-3 right-3 w-9 h-9 
               flex items-center justify-center shadow heart-pulse"
      >
        🤍
      </button>
    </div>

    <!-- CONTENT -->
    <div class="p-4">

      <!-- TYPE + VIEWS -->
      <div class="flex items-center justify-between mb-1">
        <span class="inline-flex items-center gap-1 text-xs text-green-700
                     border border-green-200 rounded-full px-2 py-0.5 bg-green-50">
          <span class="w-2 h-2 bg-green-600 rounded-full"></span>
          {{ typeLabel }}
        </span>

        <span class="text-gray-500 text-xs flex items-center gap-1">
          👁 2.3K
        </span>
      </div>

      <!-- PRICE + DETAILS -->
      <div class="flex items-center justify-between mt-1">
        <div class="text-lg font-bold text-[#0A5FD8]">$3,349,000</div>

        <div class="flex gap-4 text-sm text-gray-600">
          <span><b>4</b> Beds</span>
          <span><b>3</b> Baths</span>
          <span><b>998</b> sqft</span>
        </div>
      </div>

      <p class="text-sm text-gray-800 mt-2">
        2856 Meadow Park Ave, Henderson, NV 89052
      </p>

      <p class="text-xs text-gray-400 mt-1">MLS GRID</p>

    </div>
  </div>
</template>
