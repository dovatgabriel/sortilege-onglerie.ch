<script setup lang="ts">
import HeaderSection from '@/components/HeaderSection.vue';
import SocialSection from '@/components/SocialSection.vue';
</script>

<template>
  <HeaderSection />
  <SocialSection />
</template>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Merriweather:ital,wght@0,300;0,400;0,700;0,900;1,300;1,400;1,700;1,900&family=Montserrat:ital,wght@0,100..900;1,100..900&display=swap');

body {
  margin: 0;
  padding: 0;
}

h1 {
  font-family: 'Merriweather', serif;
}

* {
  font-family: 'Montserrat', sans-serif;

  &::selection {
    background-color: #333;
    color: #f8f8f8;
  }
}
</style>
