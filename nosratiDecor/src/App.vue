<script setup>
import {RouterView } from 'vue-router'
// import HelloWorld from './components/HelloWorld.vue'
import Header from './components/FixHeader.vue'
import Animation from './components/FixAnimation.vue'
import Footer from './components/FixFooter.vue'
</script>

<template>
  <!-- <Header -->
    <main class="main-root">
      <div id="dsn-scrollbar">
        <div class="wrapper">
          <Header />
          <Animation />
        </div>
        <Footer />
      </div>
    </main>

    <!-- <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld msg="You did it!" />

      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>
  </header> -->

  <RouterView />
</template>

<style>
@import '@/assets/css/plugins.css';
@import '@/assets/css/style.css';
</style>
