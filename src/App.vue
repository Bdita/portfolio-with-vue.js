<template>
  <div id="app">
  <md-layout md-gutter="16">
    <md-layout md-flex="30" class='profileContainer'>
      <router-view> </router-view>
    </md-layout>
  </md-layout>
  </div>
</template>

<script>
export default {
  name: 'app',
};
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  width: 100%;
  height: 100vh;
  margin: 0px;
  padding: 0px;
}
.logo {
  width: 20%;
  margin: 2% 0 0 -65% ;
}
.profileContainer {
  margin: 10% 0 0 35%;
}
</style>
