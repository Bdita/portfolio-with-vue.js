<template>
  <div id="SideNav">
  <!-- ....................................COMMENTS......................................... -->

        <!-- SideNavDrawer for each SideNav Menu item -->
        <!-- TO DO: REFACTOR ( Add Abstraction, minimise code repetition) -->

  <!-- ......................................END............................................ -->

    <div>
      <button id="btn1" class="buttonStyle" @click="toggleRightSidenavStory">
        <h3> My Story </h3>
      </button>
      <md-sidenav class="md-right" ref="rightSidenavStory" @open="open('Right')" @close="close('Right')">
            <MyStory></MyStory>
       </md-sidenav>
    </div>

    <div>
       <button id="btn2" class="buttonStyle" @click="toggleRightSidenavSkills">
         <h3> Skills </h3>
       </button>
       <md-sidenav class="md-right" ref="rightSidenavSkills" @open="open('Right')" @close="close('Right')">
       <md-toolbar>
         <div class="md-toolbar-container">
           <h3 class="md-title">Sidenav Skills content</h3>
         </div>
       </md-toolbar>
        </md-sidenav>
    </div>
    <!-- <a href="https://www.example.co.uk">
      <div id="btn2" class="button">
        <md-button @click="toggleRightSidenav"> Skills</md-button>
      </div>
    </a>

    <a href="https://www.example.co.uk">
      <div id="btn3" class="button">
        <h3>Portfolio</h3>
      </div>
    </a>

    <a href="https://www.example.co.uk">
      <div id="btn4" class="button">
        <h3>Testimonials</h3>
      </div>
    </a>

    <a href="https://www.example.co.uk">
      <div id="btn5" class="button">
        <h3>Contact</h3>
      </div>
    </a>

    <a href="https://www.example.co.uk">
      <div id="btn6" class="button">
        <h3>ABOUT</h3>
      </div>
    </a> -->
  </div>
</template>

<script>
import MyStory from './MyStory';

export default {
  name: 'sideNav',
  methods: {
    toggleRightSidenavStory() {
      this.$refs.rightSidenavStory.toggle();
    },
    toggleRightSidenavSkills() {
      this.$refs.rightSidenavSkills.toggle();
    },
  },
  components: {
    MyStory,
  },
};
</script>

<style>
h3 {
  font-family: verdana, sans-serif;
  font-weight: bold;
  text-align: center;
  position: relative;
  top: -10px;
}

a {
  text-decoration: none;
}

#btn1 {
  margin-top: 0;
}

#btn2 {
    margin-top: 40px;
}

#btn3 {
  margin-top: 80px;
}

#btn4 {
  margin-top: 120px;
}

#btn5 {
    margin-top: 160px;
}

#btn6 {
  margin-top: 200px;
}

.buttonStyle {
  background-color: #009688;
  color: #2c3e50;
  border: none;
  width: 500px;
  height: 35px;
  position: fixed;
  left: -450px;
  transition: .7s ease;
  border-radius: 50px;
}
  .buttonStyle  h3 {
    color: #fff;
  }

.buttonStyle:hover {
  background-color: #009688;
  position: fixed;
  left: 1px;
  width: 150px;
  border-radius: 50px;
}

.buttonStyle:active {
  background-color: #E91E63;
  transition: 0s;
}



</style>
