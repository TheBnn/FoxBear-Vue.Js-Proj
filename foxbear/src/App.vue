<template>
  <MainPage/>
</template>

<script>
import MainPage from './components/main.vue'
require('./assets/css/common.css');
export default {
  name: 'App',
  components: {
    MainPage
  }
}
</script>

<style>

  body{
    margin: 0;
    padding: 0;
    outline: none;
  }
  .container{
    width: 1088px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    margin: 0 auto;
  }
</style>
