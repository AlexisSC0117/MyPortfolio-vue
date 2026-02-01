<template>
  <div class="page">
    <div class="container">
      <Sidebar />
      <MainContent />
    </div>
  </div>
</template>

<script setup>
import Sidebar from "./components/Sidebar.vue"
import MainContent from "./components/MainContent.vue"
</script>

<style>
body {
  margin: 0;
  font-family: Inter, system-ui, sans-serif;
  background: #0b1220;
  color: #e5e7eb;
}

.page {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
}

.container {
  display: grid;
  grid-template-columns: 300px 1fr;
  gap: 24px;
  width: 95%;
  max-width: 1200px;
}
</style>
