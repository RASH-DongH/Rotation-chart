<script setup lang="ts">
import { ref } from 'vue';
import Children from './Chilren.vue'
const sliders = ref<{imgUrl: string}[]>([
  {imgUrl: './assets/cos海琴烟 cosplay美女4k高清壁纸_彼岸图网.jpg'},
  {imgUrl: './assets/dm.jpg'},
  {imgUrl: './assets/hl.jpg'},
  {imgUrl: './assets/iTab-1krxrv.jpg'},
  {imgUrl: './assets/iTab-57jge1.jpg'},
  {imgUrl: './assets/iTab-57o9j5.png'},
  {imgUrl: './assets/iTab-6oe337.png'},
  {imgUrl: './assets/iTab-72q3do.jpg'}
])

const time: number = 5000

</script>

<template>
  轮播图
  <hr />
  <!-- 传一个time给子组件  来定义多少秒换一张图 -->
  <Children :sliders="sliders"></Children>
</template>

<style scoped>

</style>
