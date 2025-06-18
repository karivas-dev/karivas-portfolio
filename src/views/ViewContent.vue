<script lang="ts" setup>
import Projects from '@/components/Projects.vue'
</script>

<template>
  <div id="projects" class="mt-16 mb-10">
    <div class="flex items-center gap-6 px-6 text-stone-200 my-10">
      <div class="font-bold">
        <p class="text-4xl md:text-6xl">
          Take a
          <span class="relative text-[#e75946]">
            <img
              alt="Yellow circle"
              class="w-fit absolute right-0 -translate-y-2/2"
              src="@/assets/circle.png"
            />look at
          </span>
        </p>
        <p class="text-xl md:text-4xl">what I’ve been working on</p>
      </div>
      <hr class="flex-grow border-t border-gray-300" />
    </div>

    <div>
      <p
        class="border px-6 py-1 uppercase text-[#448ccb] border-[#448ccb] rounded-full w-fit tracking-widest mx-6"
      >
        Projects
      </p>
      <Projects class="px-6 pb-6" />
    </div>
  </div>

  <div id="contact-me" class="flex items-center gap-6 px-6 text-stone-200 mt-16 mb-10">
    <hr class="flex-grow border-t border-gray-300" />
    <div class="font-bold">
      <p class="text-4xl md:text-6xl text-end">
        Let's
        <span class="relative text-[#448ccb]">
          <img
            alt="Circle"
            class="w-fit absolute right-0 -translate-y-2/2"
            src="@/assets/circle.png"
          />
          connect
        </span>
      </p>
      <p class="text-xl md:text-4xl">and see what we can create</p>
    </div>
  </div>
</template>
