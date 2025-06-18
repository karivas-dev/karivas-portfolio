<script lang="ts" setup>
import ProjectCard from '@/components/ProjectCard.vue'
import FranWeb from '@/assets/projects/fran-web.jpeg'
import Mestizo from '@/assets/projects/mestizo.jpeg'
import WarehouseWise from '@/assets/projects/ww.png'
import Game from '@/assets/projects/game.png'

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
  <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-2 my-4">
    <template v-for="(project, index) in projects" :key="index">
      <ProjectCard :project="project" />
    </template>
  </div>
</template>
