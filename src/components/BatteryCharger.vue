<template>
  <div class="main-outer">
    <h1>Battery charger Animation</h1>
    <div class="box"></div>
  </div>
</template>

<script></script>
<style scoped>
h1 {
  color: white;
  font-weight: bold;
  font-size: 30px;
  padding-bottom: 5%;
}
.box {
  width: 150px;
  height: 80px;
  border: 3px solid whitesmoke;
  border-radius: 12px;
  position: relative;
}
.box::before {
  content: "";
  position: absolute;
  top: 50%;
  right: -10px;
  transform: translate(10px, -50%);
  width: 10px;
  height: 25px;
  background-color: transparent;
  border: 1px solid whitesmoke;
}
.box::after {
  width: 0;
  height: 100%;
  content: "";
  position: absolute;
  background: #f1efef;
  border-radius: 7px;
  animation: animate 5s linear infinite;
}
@keyframes animate {
  0% {
    width: 0%;
    background: red;
  }
  25% {
    width: 25%;
    background: orange;
  }
  50% {
    width: 50%;
    background: yellow;
  }
  75% {
    width: 75%;
    background: #d7fc03;
  }
  100% {
    width: 100%;
    background: green;
  }
}
</style>
