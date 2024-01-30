<template>
  <div class="mx-auto max-w-7xl px-4 lg:px-8">
    <AppHeader />
    <NuxtPage />
    <AppFooter />
  </div>
</template>
<script setup lang="ts">
useHead({
  title: 'Bnei Adam',
  meta: [{ name: 'description', content: 'My amazing site.' }],
  script: [
    {
      src: 'https://kit.fontawesome.com/6d91ab9cfa.js',
      async: true,
      crossorigin: 'anonymous'
    }
  ]
});
</script>
