<script setup>
import PropertyCard from './PropertyCard.vue'

import House1 from '../assets/images/House1.png'
import House2 from '../assets/images/House2.png'
import House3 from '../assets/images/House3.png'
import House4 from '../assets/images/House4.png'

const properties = [
  {
    id: 1,
    image: House1,
    typeLabel: 'House For Sale'
  },
  {
    id: 2,
    image: House2,
    typeLabel: 'Multi-Family Home Sale'
  },
  {
    id: 3,
    image: House3,
    typeLabel: 'Condo For Sale'
  },
  {
    id: 4,
    image: House4,
    typeLabel: 'House For Sale'
  }
]

</script>

<template>
  <div class="grid grid-cols-1 sm:grid-cols-2 gap-6">
    <PropertyCard
      v-for="item in properties"
      :key="item.id"
      :image="item.image"
      :typeLabel="item.typeLabel"
    />
  </div>
</template>
