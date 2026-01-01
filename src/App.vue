<template>
  <div class="min-h-screen bg-[#F7F7F7]">
    <Header />
    <FilterBar />
    <MainLayout />
  </div>
</template>

<script setup>
import Header from './components/Header.vue'
import FilterBar from './components/FilterBar.vue'
import MainLayout from './components/MainLayout.vue'
</script>
