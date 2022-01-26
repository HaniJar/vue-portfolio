<template>
  <div class="home">
    <h1 id="home-header">Haniah Jardien</h1>
    <h1 class="type">I'm <span id="text"></span></h1>
    <div class="icon-bar">
      <a
        href="https://www.linkedin.com/in/haniah-jardien-44b62520b/"
        target="_blank"
        class="linkedin"
        ><i class="fab fa-linkedin"></i
      ></a>
      <a href="https://github.com/HaniJar/" target="_blank" class="github"
        ><i class="fab fa-github"></i
      ></a>
      <a href="https://codepen.io/HaniJar" target="_blank" class="codepen"
        ><i class="fab fa-codepen"></i
      ></a>
    </div>
  </div>
</template>

<script>
export default {
  name: "Home",
  components: {},
};
const sentences = [" a Frontend Developer", " an Aspiring Fullstack Developer"];

function waitForMs(ms) {
  return new Promise((resolve) => setTimeout(resolve, ms));
}

async function typeSentence(sentence, element, delay = 100) {
  const letters = sentence.split("");
  let i = 0;
  while (i < letters.length) {
    await waitForMs(delay);
    document.querySelector(element).append(letters[i]);
    i++;
  }
}

async function deleteSentence(element) {
  const sentence = document.querySelector(element).innerHTML;
  const letters = sentence.split("");
  while (letters.length > 0) {
    await waitForMs(100);
    letters.pop();
    document.querySelector(element).innerHTML = letters.join("");
  }
}

async function sentenceLoop(sentenceList, element) {
  let i = 0;
  while (true) {
    await typeSentence(sentenceList[i], element);
    await waitForMs(1500);
    await deleteSentence(element);
    await waitForMs(500);
    i++;
    if (i >= sentenceList.length) {
      i = 0;
    }
  }
}

sentenceLoop(sentences, "#text");
</script>

<style>
.navbar {
  padding: 0px !important;
  margin-top: 25px;
  right: 15px;
}
* {
  background-color: black;
}
#home-header {
  margin-top: 180px;
  font-size: 70px;
  font-weight: 700;
  letter-spacing: 4px;
}
#text {
  position: relative;
}

#text:after {
  content: "";
  width: 2px;
  height: 70%;
  background: rgb(0, 0, 0);
  position: absolute;
  animation: blink 3s infinite;
}

@keyframes blink {
  0%,
  49% {
    background: white;
  }
  50%,
  100% {
    background: black;
  }
}
.type {
  margin-top: 20px;
  font-size: 35px;
  letter-spacing: 2px;
}
h1 {
  color: white;
}
.icon-bar {
  position: fixed;
  top: 85%;
  right: 42px;

  -webkit-transform: translateY(-50%);
  -ms-transform: translateY(-50%);
  transform: translateY(-50%);
}

.icon-bar a {
  display: block;
  text-align: center;
  padding: 5px;
  transition: all 0.3s ease;
  color: white;
  font-size: 20px;
}

.icon-bar a:hover {
  background-color: #000;
}
.content {
  margin-left: 75px;
  font-size: 30px;
}
</style>
