<script setup>
import { RouterLink } from 'vue-router'
</script>

<template>
  <header>
    <nav>
      <RouterLink to="/">
        <img src="" id="logo" />
      </RouterLink>
      <RouterLink to="/">Home</RouterLink>
      <RouterLink to="/orders">About</RouterLink>
    </nav>
  </header>
</template>

<style scoped></style>
