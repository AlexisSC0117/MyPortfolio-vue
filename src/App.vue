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
  align-items: flex-start; /* FIX: allow vertical scroll */
  padding: 20px 0;
}

.container {
  display: grid;
  grid-template-columns: 300px 1fr;
  gap: 24px;
  width: 100%;
  max-width: 1100px;
}

/* MOBILE PORTRAIT MODE */
@media (max-width: 768px) {
  .container {
    grid-template-columns: 1fr; /* stack vertically */
  }
}
</style>
