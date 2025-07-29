<script setup>
import MainPage from './components/MainPage.vue'
</script>

<template>
  <div id="app">
    <MainPage />
  </div>
</template>

<style>
#app {
  min-height: 100vh;
  width: 100vw;
  margin: 0;
  padding: 0;
  overflow-x: hidden;
  overflow-y: auto;
  position: relative;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html, body {
  margin: 0;
  padding: 0;
  width: 100vw;
  max-width: 100vw;
  overflow-x: hidden;
  font-family: "Pretendard", -apple-system, BlinkMacSystemFont, sans-serif;
  line-height: 1.6;
  color: #333;
}
</style>
