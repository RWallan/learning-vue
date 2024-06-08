<script setup>
import { RouterView } from 'vue-router'
import NavbarComponent from './components/NavbarComponent.vue'
import FooterComponent from './components/FooterComponent.vue'

const app_name = 'Make Your Burguer'
const logo = '/img/logo.png'
</script>

<template>
  <NavbarComponent :logo="logo" :alt="app_name" />
  <RouterView />
  <FooterComponent />
</template>

<style>
* {
  font-family: Helvetica;
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

.main-container {
    margin: 50px;
    min-height: 250px;
}

h1 {
    text-align: center;
    font-size: 42px;
    margin-bottom: 30px;
    color: #222
}
</style>
