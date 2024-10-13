<script setup>
import TranslateCard from '@/components/TranslateCard.vue'
import TranslatedCard from '@/components/TranslatedCard.vue'
</script>

<template>
  <main>
    <img src="@/assets/resources/logo.svg" alt="Logo" />
    <section class="container">
      <TranslateCard />
      <TranslatedCard />
    </section>
  </main>
</template>

<style scoped>
main {
  margin-top: 100px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 40px;
}

.container {
  padding: 2rem;
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  column-gap: 32px;
}
</style>
