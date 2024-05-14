<template>
  <div class="container" v-for="(item, index) in data.a" :key="index">
    <img class="image" :src="item" alt="">
  </div>
</template>

<script setup>
const data = defineProps(['a'])
console.log(data.a);

</script>

<style lang="scss" scoped>
.container {
  border: 1px solid #000;
  margin: 0 5px;
  border-radius: 10px;
  position: relative;
  overflow: hidden;

  .image {
    border-radius: 10px;
    width: 100px;
    height: 100%;
  }

  .msg {
    font-size: 18px;
    bottom: 60px;
    color: aliceblue;
    left: 60px;
    position: absolute;
  }
}
</style>