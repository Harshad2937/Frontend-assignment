<template>
  <button
    class="h-11 px-5 rounded-lg text-sm font-medium
           border border-gray-300 bg-white
           hover:border-[#0A5FD8]
           transition
           flex items-center gap-2 text-gray-800">

    <!-- Icon -->
    <span v-if="icon" class="text-gray-600">
      <template v-if="label === 'Filters'">⚙️</template>
      <template v-else>❤️</template>
    </span>

    {{ label }}

    <!-- Dropdown arrow -->
    <span v-if="!icon" class="text-xs">▼</span>
  </button>
</template>

<script setup>
defineProps({
  label: String,
  icon: Boolean
})
</script>
