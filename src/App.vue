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
  display:flex;
  justify-content: center;
  background-color:#ebeff2;
  font-family: 'Roboto', sans-serif;
  color:#686868;
  font-size:16px;
}
.text__secondary{
  color:darkgrey;
  font-size:14px;
  font-weight:200;
}
</style>
