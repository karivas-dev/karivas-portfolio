<script lang="ts" setup>
import Navigation from '@/components/Navigation.vue'
import Footer from '@/components/Footer.vue'
import Welcome from '@/components/Welcome.vue'
import ViewContent from '@/views/ViewContent.vue'
</script>

<template>
  <div class="bg-[#2f2f2f] font-poppins">
    <div id="home">
      <Navigation />
      <Welcome />
    </div>
    <ViewContent />
    <Footer />
  </div>
</template>
