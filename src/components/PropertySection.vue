<script setup>
import PropertyCard from './PropertyCard.vue'

import House1 from '../assets/images/House1.png'
import House2 from '../assets/images/House2.png'
import House3 from '../assets/images/House3.png'
import House4 from '../assets/images/House4.png'

const properties = [
  { id: 1, image: House1, typeLabel: 'House For Sale' },
  { id: 2, image: House2, typeLabel: 'Multi-family Home For Sale' },
  { id: 3, image: House3, typeLabel: 'Condo For Sale' },
  { id: 4, image: House4, typeLabel: 'House For Sale' }
]
</script>

<template>
  <div>

    <!-- HEADER -->
    <div class="mb-4">
      <div class="flex items-start justify-between">
        <div>
          <h2 class="text-lg font-semibold text-gray-900">
            Austin, TX real estate & homes for sale
          </h2>
          <p class="text-sm text-gray-500 mt-1">
            2,010 Homes
          </p>
        </div>

        <button class="text-sm text-gray-600 flex items-center gap-1">
          Sort by:
          <span class="font-medium text-[#0A5FD8]">New Listing</span> ▾
        </button>
      </div>
    </div>

    <!-- CARDS GRID -->
    <div class="grid grid-cols-1 sm:grid-cols-2 gap-6">
      <PropertyCard
        v-for="item in properties"
        :key="item.id"
        :image="item.image"
        :typeLabel="item.typeLabel"
      />
    </div>

  </div>
</template>
