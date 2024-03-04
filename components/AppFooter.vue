<template>
  <footer>
    <div class="mx-auto max-w-7xl overflow-hidden px-6 py-20 sm:py-24 lg:px-8">
      <nav class="-mb-6 sm:flex sm:justify-center sm:space-x-12" aria-label="Footer">
        <li class="btn btn-link no-underline">
          <NuxtLink :to="localPath('/')" class="btn btn-link text-yellow-500 no-underline">{{ $t('nav_home') }}</NuxtLink>
        </li>

        <li class="btn btn-link no-underline">
          <NuxtLink :to="localPath('/#about')" class="btn btn-link text-yellow-500 no-underline">{{ $t('nav_about') }}</NuxtLink>
        </li>

        <li class="btn btn-link text-yellow-500 no-underline">
          <a href="#more">{{ $t('nav_contact') }}</a>
        </li>
        <LangSwitcher />
      </nav>

      <p class="mt-10 text-center text-xs leading-5 text-gray-500">&copy; {{ $t('footer_txt') }}</p>
    </div>
  </footer>
</template>
<script setup lang="ts">
const localPath = useLocalePath();
</script>
