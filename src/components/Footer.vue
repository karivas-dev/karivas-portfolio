<script lang="ts" setup>
import { Linkedin, Mail } from 'lucide-vue-next'
import { RouterLink } from 'vue-router'
</script>

<template>
  <div class="flex justify-center items-center py-2">
    <router-link :to="{ path: '/', hash: '#home' }">
      <img alt="Logo" class="w-36" src="@/assets/logo.png" />
    </router-link>
  </div>

  <div
    class="flex flex-col md:flex-row space-y-2 text-white justify-center items-center md:divide-x-1 py-6"
  >
    <a
      class="flex space-x-2 px-3 mb-0"
      href="https://www.linkedin.com/in/karen-rivas-webdeveloper/"
      target="_blank"
    >
      <Linkedin />
      <span>Karen Rivas</span>
    </a>

    <a
      class="flex space-x-2 px-3 mb-0"
      href="mailto:karenrivasg17@gmail.com?subject=Let's create together!"
    >
      <Mail />
      <span> karenrivasg17@gmail.com </span>
    </a>

    <a class="flex px-2 space-x-2" href="https://github.com/karivas-dev">
      <svg
        class="size-6"
        fill="white"
        role="img"
        viewBox="0 0 24 24"
        xmlns="http://www.w3.org/2000/svg"
      >
        <title>GitHub</title>
        <path
          d="M12 .297c-6.63 0-12 5.373-12 12 0 5.303 3.438 9.8 8.205 11.385.6.113.82-.258.82-.577 0-.285-.01-1.04-.015-2.04-3.338.724-4.042-1.61-4.042-1.61C4.422 18.07 3.633 17.7 3.633 17.7c-1.087-.744.084-.729.084-.729 1.205.084 1.838 1.236 1.838 1.236 1.07 1.835 2.809 1.305 3.495.998.108-.776.417-1.305.76-1.605-2.665-.3-5.466-1.332-5.466-5.93 0-1.31.465-2.38 1.235-3.22-.135-.303-.54-1.523.105-3.176 0 0 1.005-.322 3.3 1.23.96-.267 1.98-.399 3-.405 1.02.006 2.04.138 3 .405 2.28-1.552 3.285-1.23 3.285-1.23.645 1.653.24 2.873.12 3.176.765.84 1.23 1.91 1.23 3.22 0 4.61-2.805 5.625-5.475 5.92.42.36.81 1.096.81 2.22 0 1.606-.015 2.896-.015 3.286 0 .315.21.69.825.57C20.565 22.092 24 17.592 24 12.297c0-6.627-5.373-12-12-12"
        />
      </svg>
      <span class="text-nowrap">karivas-dev</span>
    </a>
  </div>

  <footer>
    <div class="w-full max-w-screen-xl mx-auto pb-6">
      <hr class="my-6 border-gray-300 sm:mx-auto lg:mb-8" />
      <span class="block text-sm text-gray-500 text-center dark:text-gray-400"
        >© 2025 <a class="hover:underline" href="https://github.com/karivas-dev">karivas-dev</a>.
        All Rights Reserved.</span
      >
    </div>
  </footer>
</template>
