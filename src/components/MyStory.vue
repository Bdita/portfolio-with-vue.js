<template>
  <div class='myStory'>
      <h3 data-content=''>My Story</h3>
      <div class='cards-container'>
          <p> Hello </p>
      </div>
  </div>
</template>

<script>
export default {
  name: 'myStory',
};
</script>

<!-- Add 'scoped' attribute to limit CSS to this component only -->
<style scoped>
  .myStory {
    font-family: 'Archivo Black', sans-serif;
    margin-top: -2%;
  }
  .cards-container {
    width: 98%;
    margin: 1%;
    font-family: 'Zilla Slab', serif;
    font-size: 20px;
    border: 1px solid red;
  }

  h3 {
    font-family: 'Archivo Black', sans-serif;
    font-size: 25px;
    font-weight: normal;
    position: relative;
    color: #fff;
  }

  h3:after {
    content: '';
    position: absolute;
    color: #fff;
    top: 70%;
    left: 39.5%;
    width: 21%;
    height: 70%;
    background-color: #300e5f;
    z-index: -10;
  }

  .animated-paragraph {

  }

</style>
