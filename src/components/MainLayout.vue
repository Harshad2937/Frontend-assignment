<script setup>
import MapSection from './MapSection.vue'
import PropertyList from './PropertyList.vue'
</script>

<template>
  <div class="grid grid-cols-12 h-[calc(100vh-140px)]">

    <!-- MAP (smaller) -->
    <div class="col-span-12 lg:col-span-5 border-r">
      <MapSection />
    </div>

    <!-- CARDS (bigger) -->
    <div class="col-span-12 lg:col-span-7 p-6 overflow-y-auto">
      <PropertyList />
    </div>

  </div>
</template>
