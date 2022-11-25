<script setup>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
</script>

<template>
  <header>
      <AppHeader/>
  </header>
  <main>
      <AppMain/>
  </main>
  <footer>
      <AppFooter/>
  </footer>
</template>

<style lang="scss">
  @import './style/global.scss';
  body{
    font-family: 'Open Sans', sans-serif;
    font-size: 12px;
    color: white;
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
  .align-items-center{
    align-items: center;
  }
  main{
    background-color: #1c1c1c;
  }
  *{
    box-sizing: border-box;
    margin: 0;
    padding: 0;
  }
  .flex-wrap{
    flex-wrap: wrap;
  }
</style>
