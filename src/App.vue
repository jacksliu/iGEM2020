<template>
  <div id="app">
    <el-container>
      <el-header style="padding: 0">
        <Nav/>
      </el-header>
      <el-main style="padding: 0">
        <router-view/>
      </el-main>
    </el-container>
  </div>
</template>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /*text-align: center;*/
  font-size: 20px;
  color: #2c3e50;
}

body{
  padding:0 !important;
  margin:0 !important;
}
</style>

<script>
import Nav from '@/components/Nav'

export default {
  name: 'App',
  components: {
    Nav
  }
}
</script>
