<template>
  <div id="app">
    <MainPage/>
  </div>
</template>

<script>
import MainPage from './components/mainPage.vue'

export default {
  name: 'App',
  components: {
    MainPage
  }
}
</script>

<style>
#app{
  background-color:lightyellow;
}
</style>
