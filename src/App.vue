<template>
  <div class="main">
    <WelcomeItem :a="a"></WelcomeItem>
    <smallItem :a="a"></smallItem>
  </div>
</template>

<script setup>
import WelcomeItem from './components/WelcomeItem.vue'
import smallItem from './components/smallItem.vue'

import { ref } from 'vue'
const a = ref(['./src/assets/法罗群岛1.JPG', './src/assets/法罗群岛2.JPG', './src/assets/法罗群岛3.JPG', './src/assets/法罗群岛4.JPG', './src/assets/法罗群岛5.JPG'])
</script>

<style lang="scss" scoped>
.main {
  display: flex;
}
</style>
