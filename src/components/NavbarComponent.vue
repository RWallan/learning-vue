<script setup>
import { RouterLink } from 'vue-router'
defineProps(['logo', 'alt'])
</script>

<template>
  <header>
    <nav class="bg-dark d-flex justify-content-end align-items-center ps-4 pe-4 pt-2 pb-2" id="nav">
      <RouterLink to="/" id="logo-url">
        <img :src="logo" :alt="alt" id="logo" />
      </RouterLink>
      <RouterLink to="/">Home</RouterLink>
      <RouterLink to="/orders">Orders</RouterLink>
    </nav>
  </header>
</template>

<style scoped>
#nav {
  border-botom: 4px solid #111;
}

#nav a {
  text-decoration: none;
  color: #fcba03;
  margin: 12px;
  transition: 0.5s;
}

#nav a:hover {
  color: #fff;
}

#nav #logo-url {
  margin: auto;
  margin-left: 0;
}

#logo {
  width: 40px;
  height: 40px;
}
</style>
