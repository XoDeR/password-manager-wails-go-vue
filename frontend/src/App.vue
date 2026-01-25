<script lang="ts" setup>
import Home from './components/Home.vue';
import Layout from './components/Layout.vue';
</script>

<template>
  <Layout />
  <main class="main">
    <Home />
  </main>
</template>

<style>
#logo {
  display: block;
  width: 50%;
  height: 50%;
  margin: auto;
  padding: 10% 0 0;
  background-position: center;
  background-repeat: no-repeat;
  background-size: 100% 100%;
  background-origin: content-box;
}
</style>
