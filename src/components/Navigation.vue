<script lang="ts" setup>
import { RouterLink } from 'vue-router'
</script>

<template>
  <nav class="flex justify-between px-4 py-4 items-center space-x-4 text-white">
    <router-link :to="{ path: '/', hash: '#home' }">
      <img alt="Logo" class="w-24" src="@/assets/logo.png" />
    </router-link>
    <div class="space-x-4">
      <router-link :to="{ path: '/', hash: '' }">About me</router-link>
      <router-link :to="{ path: '/', hash: '#projects' }">Projects</router-link>
      <router-link :to="{ path: '/', hash: '#contact-me' }">Contact me</router-link>
    </div>
  </nav>
</template>
