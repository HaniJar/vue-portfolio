<template>
  <div class="about">
    <h1 id="about-header">About Me</h1>
    <div class="navbar-devider">
      <div class="nd-1"></div>
      <div class="nd-2"></div>
      <div class="nd-3"></div>
      <div class="nd-4"></div>
      <div class="nd-5"></div>
      <div class="nd-6"></div>
      <div class="nd-7"></div>
    </div>
  </div>
</template>

<script></script>

<style>
#about-header {
  margin-top: 60px;
  font-size: 50px;
  font-weight: 700;
  letter-spacing: 2px;
}
.navbar-devider {
  width: 8%;
  height: 4px;
  border-radius: 50px;
  background: black;
  margin-left: 598px;
  margin-right: 800px;
}
.navbar-devider div {
  width: 14.28571429%;
  height: 100%;
  float: left;
}
@keyframes nd1 {
  0% {
    width: 7%;
  }
  35% {
    width: 25%;
  }
  70% {
    width: 10%;
  }
  100% {
    width: 7%;
  }
}
@keyframes nd2 {
  0% {
    width: 24%;
  }
  35% {
    width: 11%;
  }
  70% {
    width: 8%;
  }
  100% {
    width: 24%;
  }
}
@keyframes nd3 {
  0% {
    width: 10%;
  }
  35% {
    width: 20%;
  }
  70% {
    width: 12%;
  }
  100% {
    width: 10%;
  }
}
@keyframes nd4 {
  0% {
    width: 22%;
  }
  35% {
    width: 4%;
  }
  70% {
    width: 15%;
  }
  100% {
    width: 22%;
  }
}
@keyframes nd5 {
  0% {
    width: 15%;
  }
  35% {
    width: 12%;
  }
  70% {
    width: 11%;
  }
  100% {
    width: 15%;
  }
}
@keyframes nd6 {
  0% {
    width: 17%;
  }
  35% {
    width: 5%;
  }
  70% {
    width: 24%;
  }
  100% {
    width: 17%;
  }
}
@keyframes nd7 {
  0% {
    width: 5%;
  }
  35% {
    width: 23%;
  }
  70% {
    width: 20%;
  }
  100% {
    width: 5%;
  }
}
.navbar-devider .nd-1 {
  background: rgb(218, 68, 68);
  animation: nd1 3s infinite;
}
.navbar-devider .nd-2 {
  background: rgb(212, 86, 86);
  animation: nd2 3s infinite;
}
.navbar-devider .nd-3 {
  background: rgb(209, 105, 105);
  animation: nd3 3s infinite;
}
.navbar-devider .nd-4 {
  background: rgb(204, 125, 125);
  animation: nd4 3s infinite;
}
.navbar-devider .nd-5 {
  background: rgb(204, 143, 143);
  animation: nd5 3s infinite;
}
.navbar-devider .nd-6 {
  background: rgb(194, 159, 159);
  animation: nd6 3s infinite;
}
.navbar-devider .nd-7 {
  background: rgb(197, 179, 179);
  animation: nd7 3s infinite;
}
</style>
