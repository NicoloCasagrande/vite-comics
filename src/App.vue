<script setup>
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
</script>

<template>
  <header>
      <AppHeader/>
  </header>
  <main>
      <AppMain/>
  </main>
  <footer>
    
  </footer>
</template>

<style lang="scss">
  // @import './style/global.scss';
  body{
    font-family: 'Open Sans', sans-serif;
    font-size: 12px;
  }
  .container{
    max-width: 75rem;
    margin: auto;
    align-items: center;
  }
  .flex{
    display: flex;
  }
  .column{
    flex-direction: column;
  }
  .space-between{
    justify-content: space-between;
  }
</style>
