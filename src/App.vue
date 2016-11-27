<template>
  <div id="app">
    <my-header></my-header>
      <div class="main">
        <keep-alive>
          <router-view></router-view>
        </keep-alive>
      </div>
    <my-footer></my-footer>
  </div>
</template>

<script>
import MyHeader from './components/header'
import MyFooter from './components/footer'

export default {
  name: 'app',
  components: {
    MyHeader, MyFooter
  }
}
</script>

<style>
body{
  margin:0;
  padding:0;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
.main{
  height:500px;
}
</style>
