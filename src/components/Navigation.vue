<script lang="ts" setup>
import { RouterLink } from 'vue-router'
</script>

<template>
  <nav class="flex justify-between px-4 py-4 items-center space-x-4 text-white">
    <router-link :to="{ path: '/', hash: '#home' }">
      <img alt="Logo" class="w-24" src="@/assets/logo.png" />
    </router-link>
    <div class="divide-x-1 text-sm md:text-base">
      <router-link :to="{ path: '/', hash: '#about-me' }" class="px-1 md:px-2"
        >About me
      </router-link>
      <router-link :to="{ path: '/', hash: '#projects' }" class="px-1 md:px-2"
        >Projects
      </router-link>
      <router-link :to="{ path: '/', hash: '#contact-me' }" class="px-1 md:px-2"
        >Contact
      </router-link>
    </div>
  </nav>
</template>
