<template>
  <div id="app">
  <md-layout>
    <md-layout class='typer-container'>
      <vue-typer text='< bandit of code />'
      :pre-type-delay=70
      :type-delay=70
      :pre-erase-delay=2000
      :erase-delay=250
      eraseStyle='select-back'
      caret-animation='blink'></vue-typer>
    </md-layout>
    <md-layout class='action-container'>
      <md-button class="md-raised md-accent">Hire Me</md-button>
    </md-layout>
  </md-layout>
    <md-layout md-gutter="16">
      <div class="arrow bounce">
        <i class="material-icons">keyboard_arrow_down</i>
      </div>
      <md-layout md-flex="5"class='sidenav-container'>
        <SideNav> </SideNav>
      </md-layout>
      <md-layout md-flex="30" class='profile-container'>
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
body {
  overflow-x: hidden;
  overflow-y: hidden;
}

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
.typer-container {
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
.action-container {
  margin: 2.5% 10% 4% 40%;
}
.sidenav-container {
  margin: 10% 0% 0% 0%;
}
.profile-container {
  margin: 10% 0 0 30%;
}
.arrow {
  position: fixed;
  bottom: 53%;
  margin-left: 5px;
  width: 40px;
  height: 40px;
  color: #E91E63;
}
.bounce {
    -webkit-animation: bounce 2s infinite;
    animation: bounce 2s infinite;
}

/* Scroll down indicator (bouncing) */
@keyframes bounce {
  0%, 20%, 50%, 80%, 100% {
    transform: translateY(0); }
  40% {
    transform: translateY(-30px); }
  60% {
    transform: translateY(-15px); } }
</style>
