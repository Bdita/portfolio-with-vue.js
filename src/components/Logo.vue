<template>
  <div id="Logo">
  <md-layout md-gutter="16">
    <md-layout md-flex="30" class='profileContainer'>

    </md-layout>
  </md-layout>
  <vue-typer text='Hello World! I was registered locally!'></vue-typer>
  <!-- <md-layout md-gutter="16">
    <md-layout md-flex="30" class='profileContainer'>
      <router-view> </router-view>
    </md-layout>
  </md-layout> -->
  </div>
</template>

<script>
export default {
  name: 'logo',
};
</script>

<style>
.logo {
  width: 20%;
  margin: 2% 0 0 -65% ;
}
</style>
