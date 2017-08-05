<template>
  <div class="Profile ">
    <img src="http://res.cloudinary.com/dihqhbf9i/image/upload/e_art:incognito/v1501820072/11951142_10206755264775458_2690845586774658783_n_xgjsn9.jpg" class='img-circle'>
    <h3> {{ name.toUpperCase() }} </h3>
    <hr>
    <h4 class="profile-title">{{ title.toUpperCase() }}</h4>
  </div>
</template>

<script>
export default {
  name: 'profile',
  data() {
    return {
      title: 'Full-Stack Web Developer',
      name: 'Bandita Sharma',
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.Profile {
  margin: 0 0 0 0%;
}
h3 {
  color: #313640;
  font-size: 15px;
}
h4 {
  margin-top: 0%;
  font-weight: 500;
}
hr {
  width: 60px;
  margin-top: -2%;
  border: 1.5px solid #41B883;
}
.img-circle {
   border-radius: 50%;
   width: 40%;
   box-shadow: 0 0 5px rgba(0, 0, 0, 0.6)
}
</style>
