<script setup lang="ts">
import BusinessComponent from '@/components/BusinessComponent.vue'
import PhoneGiftsContainer from '@/components/PhoneGiftsContainer.vue'
</script>

<template>
  <main class="main-container">
    <BusinessComponent />
    <PhoneGiftsContainer />
  </main>
</template>

<style lang="scss" scoped>
.main-container {
  display: flex;
  flex-direction: column;
  gap: 3rem;
}
</style>
