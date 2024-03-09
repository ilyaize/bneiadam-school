<template>
  <div class="mx-auto max-w-7xl px-4 lg:px-8">
    <AppHeader />
    <NuxtPage />
    <AppFooter />
  </div>
</template>
<script setup lang="ts">
useHead({
  title: 'Bnei Adam בני אדם',
  meta: [
    { hid: 'description', name: 'description', content: 'Bnei Adam School of Osteopathy & Psychology based in Jerusalem.' },
    { hid: 'og:title', property: 'og:title', content: 'Bnei Adam בני אדם' },
    { hid: 'og:url', property: 'og:url', content: 'https://www.bneiadam.com/' },
    { hid: 'og:description', property: 'og:description', content: 'Bnei Adam School of Osteopathy & Psychology based in Jerusalem.' },
    { hid: 'og:image', property: 'og:image', content: 'https://www.bneiadam.com/_nuxt/image.9p4FlD-T.jpg' },
    { name: 'keywords', content: 'Bnei Adam School, Bnei Adam, Osteopathy, Osteopath, Psychology, Psychologist, Jerusalem' }
    // // twitter card
    // { hid: "twitter:title", name: "twitter:title", content: this.pageTitle },
    // { hid: "twitter:url", name: "twitter:url", content: this.pageUrl },
    // { hid: 'twitter:description', name: 'twitter:description', content: this.description },
    // { hid: "twitter:image", name: "twitter:image", content: process.env.baseUrl + ogImage},
  ],
  script: [
    {
      src: 'https://kit.fontawesome.com/6d91ab9cfa.js',
      async: true,
      crossorigin: 'anonymous'
    }
  ]
});
</script>
