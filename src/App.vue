<template>
  <div id="app">
  <md-layout>
    <md-layout class='typeContainer'>
      <vue-typer text='< bandit of code />'
      pre-type-delay='70'
      type-delay='70'
      pre-erase-delay='2000'
      erase-delay='250'
      eraseStyle='select-back'
      caret-animation='blink'></vue-typer>
    </md-layout>
    <md-layout class='actionContainer'>
      <md-button class="md-raised md-accent">Hire Me</md-button>
    </md-layout>
  </md-layout>
    <md-layout md-gutter="16">
      <md-layout md-flex="5"class='sideNavContainer'>
        <SideNav> </SideNav>
      </md-layout>
      <md-layout md-flex="30" class='profileContainer'>
        <router-view> </router-view>
      </md-layout>
    </md-layout>
  </div>
</template>

<script>
import SideNav from './components/SideNav';

export default {
  name: 'app',
  components: {
    SideNav,
  },
};
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  height: 100vh;
  margin: 0px;
  padding: 0px;
}
.typeContainer {
  margin: 2.5% 10% 0% 10%;
  font-family: 'Londrina Shadow', cursive;
  font-size: 1.50em;
  font-weight: bold;
  line-height: 1.75em;
  letter-spacing: 2px;
}
.vue-typer .custom.char.typed {
  color: #009688;
}
.vue-typer .custom.char.selected {
  color: #E91E63;
}
.vue-typer .custom.caret {
  animation: 1s ease-in-out 0s infinite;
}
.vue-typer .custom.caret.typing {
  background-color: #009688;
}
.vue-typer .custom.caret.selecting {
  display: inline-block;
  background-color: #E91E63;
}
.md-button {
  padding: 0% 10% 0% 10%;
  font-size: 1em;
  font-weight: bold;
  margin: 2% 0 0 35%;
  box-shadow: none;
}
.actionContainer {
  margin: 2.5% 10% 4% 30%;
}
.sideNavContainer {
  margin: 10% 0% 0% 0%;
}
.profileContainer {
  margin: 10% 0 0 30%;
}
</style>
