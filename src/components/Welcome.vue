<script lang="ts" setup>
import { ArrowDown } from 'lucide-vue-next'
</script>

<template>
  <div class="text-stone-100 h-[calc(100vh-68px)] grid place-content-center space-y-6">
    <p class="text-ms md:text-lg text-center font-extralight w-6/7 md:w-2/3 mx-auto">
      Hey! Thanks for stopping by. I'm a web developer with experience across both frontend and
      backend technologies. I love building creative, and user-friendly web experiences.
    </p>

    <div class="flex text-2xl md:text-4xl font-bold justify-center overflow-clip gap-2">
      <h1>I really enjoy</h1>
      <div class="relative text-center w-[8ch]">
        <p class="invisible">developing</p>

        <p class="absolute left-0 top-0 animate-text-slide delay-0">developing</p>
        <p class="absolute left-0 top-0 animate-text-slide delay-1">creating</p>
        <p class="absolute left-0 top-0 animate-text-slide delay-2">learning</p>
      </div>
    </div>

    <div class="translate-y-[450%]">
      <router-link to="#about-me">
        <ArrowDown class="size-8 animate-bounce place-self-center" />
      </router-link>
    </div>
  </div>

  <div
    id="about-me"
    class="min-h-screen grid grid-cols-1 lg:grid-cols-2 place-items-center space-y-12 p-2"
  >
    <div
      class="w-full md:w-2/3 lg:w-4/5 text-white mt-10 text-center lg:text-end lg:ml-auto space-y-8 lg:mr-8"
    >
      <h1 class="text-stone-100 text-4xl font-bold">Welcome!</h1>
      <p class="font-extralight">
        I’m a big fan of binge-watching series, and I’m always hungry (just not for cooking). If I’m
        not coding, I’m probably gaming with friends or finding a new experience.
      </p>
    </div>

    <div
      class="relative w-3/4 md:w-4/7 lg:w-5/8 pb-1 block lg:mr-auto lg:border-s-1 lg:border-stone-50 md:ps-10"
    >
      <p class="absolute top-2 left-14 font-extrabold text-5xl text-[#448ccb] text-shadow-lg">
        oi!
      </p>
      <img alt="Circle" class="w-full rounded-full mb-6" src="@/assets/me.jpg" />
      <div class="absolute bottom-0 right-0 leading-0 text-end text-shadow-lg">
        <p class="text-white text-xl">I am</p>
        <p class="font-bold text-6xl text-[#4e4d4d]">
          <span class="text-[#fbc106]">ka</span>ren <span class="text-[#fbc106]">rivas</span>
        </p>
      </div>
    </div>
  </div>
</template>
