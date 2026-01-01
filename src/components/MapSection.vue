<script setup>
import { onMounted } from 'vue'
import L from 'leaflet'

// Fix marker icon issue in Vite
import icon from 'leaflet/dist/images/marker-icon.png'
import iconShadow from 'leaflet/dist/images/marker-shadow.png'

const DefaultIcon = L.icon({
    iconUrl: icon,
    shadowUrl: iconShadow,
    iconSize: [25, 41],
    iconAnchor: [12, 41]
})

L.Marker.prototype.options.icon = DefaultIcon

onMounted(() => {
    const map = L.map('map').setView([37.8, -96], 4) // USA center

    // OpenStreetMap tiles
    L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
        attribution: '© OpenStreetMap'
    }).addTo(map)

    // Dummy house markers (Houzeo-style)
    const locations = [
        [34.05, -118.24], // LA
        [29.76, -95.36],  // Houston
        [40.71, -74.00],  // New York
        [41.88, -87.63],  // Chicago
        [25.76, -80.19],  // Miami
        [33.44, -112.07], // Phoenix
    ]

    locations.forEach(loc => {
        L.marker(loc).addTo(map)
    })
})
</script>

<template>
    <div class="w-full h-full rounded-2xl overflow-hidden  ">
        <div id="map" class="w-full h-full"></div>
    </div>
</template>
