<template>
  <div class='my-story'>
      <h3 data-content=''>My Story</h3>
      <div class='para-container'>
          <p> Hello </p>
      </div>
  </div>
</template>

<script>
export default {
  name: 'my-story',
};
</script>

<!-- Add 'scoped' attribute to limit CSS to this component only -->
<style scoped>
  .my-story {
    font-family: 'Archivo Black', sans-serif;
    margin-top: -2%;
  }
  .para-container {
    width: 98%;
    margin: 1%;
    font-family: 'Zilla Slab', serif;
    font-size: 20px;
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
</style>
