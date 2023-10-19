<script setup>
import Nav from './components/navbar/navbar.vue'
import Footer from './components/footer/footer.vue'
</script>

<template>
  <header>
    <Nav />
  </header>

  <RouterView />

  <footer>
    <Footer />
  </footer>
</template>
