<script setup>
import { ref } from 'vue'

const num = ref(1) //
console.log(num) // 呈現 num 渲染出來的 object
console.log(num.value) // 取得 num 的值

function clickMe() {
  num.value++
}
</script>

<template>
  <div id="app">
    {{ num }}
    <button type="button" v-on:click="clickMe">點我</button>
    <!-- 改由 btn 來觸發++ -->
    <!-- 使用 v-on 監聽，作動時觸發函式(這邊是點擊後觸發) -->
  </div>
</template>

<style scoped></style>
