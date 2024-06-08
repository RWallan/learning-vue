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
</style>
