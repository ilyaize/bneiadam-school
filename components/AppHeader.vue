<template>
  <header>
    <!-- Navigation Bar -->
    <nav class="navbar">
      <div class="flex-1 py-5">
        <NuxtLink class="flex items-center justify-center" :to="localPath('/')">
          <img src="../assets/logo.svg" class="h-12" />
          <!-- TODO: temp fix -->
          <!-- <span class="px-5 font-bold text-xl">{{ $t('home') }}</span> -->
          <div class="px-5 pt-2 text-center">
            <span class="block text-xl font-bold leading-4 text-yellow-50">{{ $t('home') }}</span>
            <span class="block text-sm tracking-widest text-yellow-500">&mdash; {{ $t('home2') }} &mdash;</span>
          </div>
        </NuxtLink>
      </div>

      <!-- navlinks -->
      <div class="hidden md:flex">
        <ul class="menu-horizontal p-0">
          <li class="btn btn-link text-yellow-500 no-underline">
            <NuxtLink :to="localPath('/')">{{ $t('nav_home') }}</NuxtLink>
          </li>

          <li class="btn btn-link text-yellow-500 no-underline">
            <NuxtLink :to="localPath('/#about')">{{ $t('nav_about') }}</NuxtLink>
          </li>

          <li class="btn btn-link text-yellow-500 no-underline">
            <a href="#more">{{ $t('nav_contact') }}</a>
          </li>

          <LangSwitcher />

          <a href="tel:+972555694652" class="btn btn-primary mx-4 border-0 bg-yellow-500 hover:bg-yellow-400">
            <i class="fa-solid fa-phone"></i>
            055-569-4652
          </a>
        </ul>
      </div>
      <!-- hamburger menu -->
      <div class="flex md:hidden">
        <div id="nav-icon3" @click="toggleNav" :class="{ open: isMenuVisible }">
          <span></span>
          <span></span>
          <span></span>
          <span></span>
        </div>
      </div>
    </nav>

    <!-- hidden navlinks -->
    <div v-show="isMenuVisible" class="flex justify-center md:hidden">
      <div class="menu-vertical space-y-3 pt-4">
        <NuxtLink :to="localPath('/')" class="btn btn-link text-yellow-500 no-underline">
          {{ $t('nav_home') }}
        </NuxtLink>
        <NuxtLink :to="localPath('/#about')" class="btn btn-link text-yellow-500 no-underline">
          {{ $t('nav_about') }}
        </NuxtLink>
        <li class="btn btn-link text-yellow-500 no-underline">
          <a href="#more">{{ $t('nav_contact') }}</a>
        </li>
        <LangSwitcher />
        <button class="btn btn-primary mx-4 border-0 bg-yellow-500 hover:bg-yellow-400">
          <i class="fa-solid fa-phone"></i>
          054-461-9687
        </button>
      </div>
    </div>
  </header>
</template>

<script setup>
import { ref, onMounted } from 'vue';

const isDarkTheme = ref(false);

onMounted(() => {
  // Initialize the theme based on a condition or default
  const defaultTheme = 'dark'; // or 'dark'
  document.documentElement.setAttribute('data-theme', defaultTheme);
  isDarkTheme.value = defaultTheme === 'dark';
});

const localPath = useLocalePath();

const isMenuVisible = ref(false);

const toggleNav = () => {
  isMenuVisible.value = !isMenuVisible.value;
};
</script>

<style lang="scss" scoped>
#nav-icon3 {
  width: 60px;
  height: 45px;
  position: relative;
  transform: rotate(0deg);
  transition: 0.5s ease-in-out;
  cursor: pointer;
}

#nav-icon3 span {
  display: block;
  position: absolute;
  height: 9px;
  width: 100%;
  background: #eab308;
  border-radius: 9px;
  opacity: 1;
  left: 0;
  transform: rotate(0deg);
  transition: 0.25s ease-in-out;
}

#nav-icon3 span:nth-child(1) {
  top: 0px;
}

#nav-icon3 span:nth-child(2),
#nav-icon3 span:nth-child(3) {
  top: 18px;
}

#nav-icon3 span:nth-child(4) {
  top: 36px;
}

#nav-icon3.open span:nth-child(1) {
  top: 18px;
  width: 0%;
  left: 50%;
}

#nav-icon3.open span:nth-child(2) {
  transform: rotate(45deg);
}

#nav-icon3.open span:nth-child(3) {
  transform: rotate(-45deg);
}

#nav-icon3.open span:nth-child(4) {
  top: 18px;
  width: 0%;
  left: 50%;
}
</style>
