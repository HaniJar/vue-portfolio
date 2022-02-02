<template>
  <div class="contact">
    <h1 id="contact-header">Contact Me</h1>
    <div class="navbar-devider">
      <div class="nd-1"></div>
      <div class="nd-2"></div>
      <div class="nd-3"></div>
      <div class="nd-4"></div>
      <div class="nd-5"></div>
      <div class="nd-6"></div>
      <div class="nd-7"></div>
    </div>
    <div class="row">
      <div id="col1" class="col-6">
        <div class="container1">
          <h3 id="message-me">Message Me</h3>
          <form action="https://formspree.io/f/mlezjnaz" method="POST">
            <ul>
              <label for="name"></label>
              <input
                type="text"
                id="name"
                name="user_name"
                placeholder="Name"
              />

              <label for="mail"></label>
              <input
                type="email"
                id="mail"
                name="user_email"
                placeholder="Email"
              />

              <li>
                <label for="msg"></label>
                <textarea rows="4" cols="21" placeholder="Message"></textarea>
              </li>
              <li>
                <button class="butt-on" type="submit">Send Message</button>
              </li>
            </ul>
          </form>
        </div>
      </div>

      <div class="col-4">
        <h3 id="contact-info">Contact Info</h3>
        <h5 id="words">Feel free to contact me!</h5>
        <div class="info">
          <h4><i class="fas fa-signature"></i> Name:</h4>
          <p>Haniah Jardien</p>
          <hr />
          <h4><i class="fas fa-map-marker-alt"></i> Location:</h4>
          <p>Cape Town, South Africa</p>
          <hr />
          <h4><i class="fas fa-phone-alt"></i> Call Me:</h4>
          <p>065 936 5051</p>
          <hr />
          <h4><i class="fas fa-envelope"></i> Email Me:</h4>
          <p>jardienhaniah@gmail.com</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script></script>

<style>
#contact-header {
  margin-top: 60px;
  font-size: 50px;
  font-weight: 700;
  letter-spacing: 2px;
}

.butt-on {
  font-family: sans-serif;
  background-color: rgb(211, 90, 110);
  color: white;
  font-weight: 400;
  font-size: 16px;
  border-radius: 30px;
  height: 40px;
  margin-top: 10px;
  border-style: solid;
  border-color: rgb(211, 90, 110);
  margin-left: -234px;
}
body {
  overflow-x: hidden;
}

ul {
  list-style: none;
  margin: 0;
  padding: 0;
}

form {
  /* background-color: #130f0f; */
  padding-top: -100px;
  padding-right: 40px;
  padding-bottom: 40px;
  padding-left: 40px;
  /* box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1); */
  border-radius: 3px;
  margin-left: -200px;
  margin-top: -1px;
}

input,
textarea {
  border: black;
  margin: 15px !important;
  padding: 9px 20px;
  border: 1px solid #000000;
  background-color: #fff;
  color: #000000;
  caret-color: #101418;
  box-sizing: border-box;
  font-size: 14px;
  font-size: 1rem;
  line-height: 29px;
  line-height: 2rem;
  box-shadow: inset 0 2px 4px 0 rgba(7, 8, 8, 0.2);
  border-radius: 3px;
  line-height: 29px;
  line-height: 2rem;
}
.navbar-devider {
  width: 8%;
  height: 4px;
  border-radius: 50px;
  background: black;
  margin-inline: auto;
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
#message-me {
  text-align: left;
  margin-left: 55px;
  color: white;
  font-family: sans-serif;
  font-weight: bold;
}
#contact-info {
  text-align: left;
  color: white;
  font-family: sans-serif;
  font-weight: bold;
}
.col-4 {
  color: rgb(128, 127, 127);
  text-align: left;
  font-size: 18px;
}
.vl {
  border-left: 2px solid rgba(116, 116, 116, 0.541);
  height: 300px;
  margin-left: 100px;
  margin-top: 25px;
}
.info {
  color: white;
}
#words {
  margin-top: 10px;
  margin-bottom: 15px;
}
</style>
