<script lang="ts" setup>
import { RouterView } from 'vue-router'
import ProjectCard from '@/components/ProjectCard.vue'
import FranWeb from '@/assets/projects/fran-web.jpeg'
import Mestizo from '@/assets/projects/mestizo.jpeg'
import Game from '@/assets/projects/game.png'
import WarehouseWise from '@/assets/projects/ww.png'
import Greeting from '@/components/Greeting.vue'
import Navigation from '@/components/Navigation.vue'
import Footer from '@/components/Footer.vue'

const projects = [
  {
    title: 'Francisco - Web',
    description:
      'Developed a responsive web portfolio for graphic designer Francisco, faithfully translating\n' +
      '        his original design into a user-friendly website with consistent behavior and layout across\n' +
      '        all devices.',
    tools: [
      {
        name: 'VueJs',
        color: '#42b883',
      },
      {
        name: 'TailwindCSS',
        color: '#00bcff',
      },
      {
        name: 'SwiperJS',
        color: '#0092ff',
      },
    ],
    url: 'https://karivas-dev.github.io/francisco-web/#/',
    img: FranWeb,
    default: false,
  },
  {
    title: 'Mestizo',
    description:
      'Developed the promotional website for Mestizo Exprés, a canned coffee brand. The site highlights the brand’s identity, showcases its products, and connects with its audience.',
    tools: [
      {
        name: 'VueJs',
        color: '#42b883',
      },
      {
        name: 'TailwindCSS',
        color: '#00bcff',
      },
      {
        name: 'SwiperJS',
        color: '#0092ff',
      },
    ],
    url: 'https://karivas-dev.github.io/mestizoWeb/',
    img: Mestizo,
    default: true,
  },
  {
    title: 'WarehouseWise',
    description:
      'WarehouseWise is an academic project built with Laravel, Vue.js, and MySQL for managing enterprise-level inventory across multiple branches. It includes features for stock control, multi-branch tracking, and centralized data access, simulating a scalable real-world inventory solution.',
    tools: [
      {
        name: 'Laravel',
        color: '#f53003',
      },
      {
        name: 'VueJs',
        color: '#42b883',
      },
      {
        name: 'MySQL',
        color: '#e48e00',
      },
    ],
    url: 'https://github.com/karivas-dev/WarehouseWise',
    img: WarehouseWise,
    default: false,
  },
  {
    title: 'HeyKiddo - JugandoAndo',
    description:
      'JugandoAndo (formerly known as HeyKiddo) is an educational video game for children, developed in Unity using C#. Created for a competition, the game introduces the basics of Intellectual Property through playful elements inspired by Salvadoran popular culture.',
    tools: [
      {
        name: 'Unity',
        color: '#4b4b4b',
      },
      {
        name: 'C#',
        color: '#641f74',
      },
    ],
    url: 'https://bocchiko.itch.io/heykiddo',
    img: Game,
    default: true,
  },
]
</script>

<template>
  <div class="bg-[#2f2f2f] font-poppins">
    <Navigation />

    <div class="flex text-4xl font-bold text-stone-100 justify-center my-60">
      <h1>I really enjoy</h1>
      <div class="relative">
        <p class="absolute animate-text-slide delay-0">developing</p>
        <p class="absolute animate-text-slide delay-1">creating</p>
        <p class="absolute animate-text-slide delay-2">learning</p>
      </div>
    </div>

    <div id="home" class="h-screen flex flex-col justify-center items-center p-2">
      <Greeting />

      <div class="w-full md:w-2/3 lg:w-3/5 text-white space-y-5 mt-10 text-center">
        <p class="">
          Hey! Thanks for stopping by. I'm a web developer with experience across both frontend and
          backend technologies. I love building creative, and user-friendly web experiences.
        </p>
        <p>
          I’m a big fan of binge-watching series, and I’m always hungry (just not for cooking). If
          I’m not coding, I’m probably gaming with friends or flipping pages in a new book.
        </p>
      </div>
    </div>

    <div id="projects" class="flex items-center gap-6 px-6 text-stone-200 my-10">
      <div class="font-bold">
        <p class="text-6xl">
          Take a
          <span class="relative text-[#e75946]">
            <img class="w-fit absolute right-0 -translate-y-2/2" src="@/assets/circle.png" />look at
          </span>
        </p>
        <p class="text-4xl">what I’ve been working on</p>
      </div>
      <hr class="flex-grow border-t border-gray-300" />
    </div>

    <p
      class="border px-6 py-1 uppercase text-[#448ccb] border-[#448ccb] rounded-full w-fit tracking-widest mx-6"
    >
      Projects
    </p>

    <div id="projects" class="px-6 pb-6">
      <div class="grid grid-cols-1 md:grid-cols-3 lg:grid-cols-4 gap-2 my-4">
        <template v-for="(project, index) in projects" :key="index">
          <ProjectCard :project="project" />
        </template>
      </div>
    </div>

    <div id="contact-me" class="flex items-center gap-6 px-6 text-stone-200 my-10">
      <hr class="flex-grow border-t border-gray-300" />
      <div class="font-bold">
        <p class="text-6xl text-end">
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
        <p class="text-4xl">and see what we can create</p>
      </div>
    </div>
    <Footer />
  </div>

  <RouterView />
</template>
