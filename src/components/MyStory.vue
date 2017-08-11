<template>
  <div class="myStory">
      <h3 data-content="">My Story</h3>
      <div class='cards-container'>
        <p> Test </p>
      </div>
  </div>
</template>

<script>
export default {
  name: 'myStory',
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .myStory {
    font-family: 'Archivo Black', sans-serif;
    margin-top: 10%;
  }
  .cards-container {
    width: 50%;
    margin: 10% 0 0 5%;
  }
  .whiteCard .md-card {
    color: #000000;
    background-color: #fff;
    position: relative;
  }
  .purpleCard .md-card {
    margin: -5% -80% 0 80%;
    background-color: #300e5f;
    z-index: 1;
  }

  h3 {
    font-family: 'Archivo Black', sans-serif;
    font-size: 30px;
    font-weight: normal;
    position: relative;
    color: #fff;
  }

  h3:after {
    content: "";
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
