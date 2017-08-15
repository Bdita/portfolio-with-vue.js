<template>
  <div id="sidenav">
  <!-- ....................................COMMENTS......................................... -->

        <!-- SideNavDrawer for each SideNav Menu item -->
        <!-- TO DO: 1. Make Vue component for each side nav item and render -->
        <!-- TO DO: 2. REFACTOR ( Add Abstraction, minimise code repetition) -->

  <!-- ......................................END............................................ -->

    <div>
      <button id="btn1" class="button-style" @click="toggleRightSideNavStory">
        <h3> My Story </h3>
      </button>
      <div>
        <md-sidenav class="md-right" ref="rightSideNavStory" @close="close('Right')">
        <span class="close-button">
          <md-button class="md-icon-button right-corner" @click="closeRightSideNavStory">
            <md-icon>close</md-icon>
          </md-button>
        </span>
            <MyStory></MyStory>
         </md-sidenav>
      </div>
    </div>

    <!-- ................................TO DO.................................
    <div>
       <button id="btn2" class="buttonStyle" @click="toggleRightSidenavSkills">
         <h3> Skills </h3>
       </button>
       <div>
         <md-sidenav class="md-right" ref="rightSidenavSkills">
           <md-toolbar>
             <div class="md-toolbar-container">
               <h3 class="md-title">Sidenav Skills content</h3>
             </div>
           </md-toolbar>
         </md-sidenav>
        </div>
    </div>

    <div>
       <button id="btn3" class="buttonStyle" @click="toggleRightSidenavPortfolio">
         <h3> Portfolio </h3>
       </button>
       <div>
         <md-sidenav class="md-right" ref="rightSidenavPortfolio">
           <md-toolbar>
             <div class="md-toolbar-container">
               <h3 class="md-title">Sidenav Portfolio content</h3>
             </div>
           </md-toolbar>
         </md-sidenav>
        </div>
    </div>

    <div>
       <button id="btn4" class="buttonStyle" @click="toggleRightSidenavTestimonials">
         <h3> Testimonials </h3>
       </button>
       <div>
         <md-sidenav class="md-right" ref="rightSidenavTestimonials">
           <md-toolbar>
             <div class="md-toolbar-container">
               <h3 class="md-title">Sidenav Testimonials content</h3>
             </div>
           </md-toolbar>
         </md-sidenav>
        </div>
    </div>

    <div>
       <button id="btn5" class="buttonStyle" @click="toggleRightSidenavContact">
         <h3> Contact </h3>
       </button>
       <div>
         <md-sidenav class="md-right" ref="rightSidenavContact">
           <md-toolbar>
             <div class="md-toolbar-container">
               <h3 class="md-title">Sidenav Contact content</h3>
             </div>
           </md-toolbar>
         </md-sidenav>
        </div>
    </div>

    <div>
       <button id="btn6" class="buttonStyle" @click="toggleRightSidenavResume">
         <h3> Resume </h3>
       </button>
       <div>
         <md-sidenav class="md-right" ref="rightSidenavResume">
           <md-toolbar>
             <div class="md-toolbar-container">
               <h3 class="md-title">Sidenav Resume content</h3>
             </div>
           </md-toolbar>
         </md-sidenav>
        </div>
    </div> ................................................................... -->
  </div>
</template>

<script>
import MyStory from './MyStory';

export default {
  name: 'SideNav',
  methods: {
    toggleRightSideNavStory() {
      this.$refs.rightSideNavStory.open();
    },
    closeRightSideNavStory() {
      this.$refs.rightSideNavStory.close();
    },
    // .............. TO DO..................
    // toggleRightSidenavSkills() {
    //  this.$refs.rightSidenavSkills.toggle();
    // },
    // toggleRightSidenavPortfolio() {
    //  this.$refs.rightSidenavPortfolio.toggle();
    // },
    // toggleRightSidenavTestimonials() {
    //  this.$refs.rightSidenavTestimonials.toggle();
    // },
    // toggleRightSidenavContact() {
    //  this.$refs.rightSidenavContact.toggle();
    // },
    // toggleRightSidenavResume() {
    //  this.$refs.rightSidenavResume.toggle();
    // },
  },
  components: {
    MyStory,
  },
};
</script>

<style>
.md-sidenav .md-sidenav-content {
  width: 715px;
}

.md-sidenav .md-backdrop {
  background-color: rgba(0, 0, 0, 0);
}

.md-theme-default.md-sidenav .md-sidenav-content {
    background-color: #E91E63;
    color: rgba(255, 255, 255, .87);
    font-size: 48px;
}

.button-style h3 {
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
  margin-top: 80px;
}

/* #btn2 {
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
} */

.button-style {
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
  .button-style  h3 {
    color: #fff;
  }

.button-style:hover {
  background-color: #009688;
  position: fixed;
  left: 1px;
  width: 150px;
  border-radius: 50px;
}

.button-style:active {
  background-color: #E91E63;
  transition: 0s;
}
.close-button {
  width: 20px;
  margin-right: -90%;
}

@media (max-width: 1280px) {
  .md-sidenav .md-sidenav-content {
      width: 635px;
  }
}

@media (max-width: 1024px) {
  .md-sidenav .md-sidenav-content {
      width: 507px;
  }
}

</style>
