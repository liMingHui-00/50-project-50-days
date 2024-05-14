<template>
  <div class="container">
    <img class="image" :src="data.a[0]" alt="">
    <span class="msg">法罗群岛</span>

  </div>
</template>

<script setup>
const data = defineProps(['a'])
console.log(data.a);

</script>

<style lang="scss" scoped>
.container {
  border: 1px solid #000;
  border-radius: 10px;
  position: relative;
  overflow: hidden;

  .image {
    border-radius: 10px;
    width: 500px;
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