<template>
  <div id="SideNav">
    <a href="https://www.example.co.uk">
      <div id="btn1" class="button">
        <h3>My Story</h3>
      </div>
    </a>

    <a href="https://www.example.co.uk">
      <div id="btn2" class="button">
        <h1>TUTORIALS</h1>
      </div>
    </a>

    <a href="https://www.example.co.uk">
      <div id="btn3" class="button">
        <h1>ABOUT</h1>
      </div>
    </a>

    <a href="https://www.example.co.uk">
      <div id="btn4" class="button">
        <h1>ABOUT</h1>
      </div>
    </a>

    <a href="https://www.example.co.uk">
      <div id="btn5" class="button">
        <h1>ABOUT</h1>
      </div>
    </a>

    <a href="https://www.example.co.uk">
      <div id="btn6" class="button">
        <h1>ABOUT</h1>
      </div>
    </a>
  </div>
</template>

<script>
export default {
  name: 'sideNav',
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
  margin-top: 0%;
}

#btn2 {
    margin-top: 3%;
}

#btn3 {
  margin-top: 6%;
}

#btn4 {
  margin-top: 9%;
}

#btn5 {
    margin-top: 12%;
}

#btn6 {
  margin-top: 15%;
}

div.button {
  background-color: #009688;
  color: #2c3e50;
  border: none;
  width: 500px;
  height: 40px;
  position: fixed;
  left: -435px;
  transition: .7s ease;
}

div.button:hover {
  background-color: #009688;
  color: #ffffff;
  position: fixed;
  left: -30px;
  width: 200px;
  border-radius: 0px;
}

div.button:active {
  background-color: #D81B60;
  transition: 0s;
  color: #ecf0f1;
}
</style>
