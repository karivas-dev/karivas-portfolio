<script lang="ts" setup>
import { ArrowUpRight } from 'lucide-vue-next'

defineProps<{
  project: {
    title: string
    description: string
    tools: {
      name: string
      color: string
    }[]
    url: string
    img: string
    default: boolean
  }
}>()
</script>

<template>
  <div class="bg-stone-100 rounded-2xl flex flex-col justify-between">
    <div class="relative rounded-2xl">
      <a
        :href="project.url"
        class="bg-white rounded-full size-10 p-2 absolute right-0.5 top-0.5"
        target="_blank"
      >
        <ArrowUpRight />
      </a>

      <div class="max-h-[45vh] overflow-hidden rounded-2xl">
        <h1
          class="absolute bottom-0.5 left-0.5 bg-stone-50/5 font-bold backdrop-grayscale backdrop-blur-xs rounded-4xl m-1 px-4 py-1 text-[#2f2f2f]"
        >
          {{ project.title }}
        </h1>
        <img :src="project.img" alt="Project screenshot" class="rounded-2xl" />
      </div>
    </div>

    <div :class="project.default ? 'order-last' : 'order-first'" class="mx-4 my-3">
      <p class="py-2 text-sm font-light">
        {{ project.description }}
      </p>

      <div class="space-x-1 flex">
        <p
          v-for="(tool, index) in project.tools"
          :key="index"
          :style="{ color: tool.color, borderColor: tool.color }"
          class="border text-xs px-3 py-0.5 rounded-full w-fit"
        >
          {{ tool.name }}
        </p>
      </div>
    </div>
  </div>
</template>
