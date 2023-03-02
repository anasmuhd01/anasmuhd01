- 👋 Hi, I’m @anasmuhd01
- 👀 I’m interested in ...technology 0s and 1s 🤯
- 🌱 I’m currently learning ... full stack(html,css,js ,nodejs,mongodb)
- 💞️ I’m looking to collaborate on ...full stack web development
- 📫 How to reach me ...

<!---
anasmuhd01/anasmuhd01 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
import Vue from "vue";
import App from "./App.vue";
import Typewriter from "typewriter-effect/dist/core";
import GraphemeSplitter from "grapheme-splitter";

Vue.config.productionTip = false;

new Vue({
  render: h => h(App)
}).$mount("#app");

const innerdemo = document.getElementById("inner-demo-2");

const stringSplitter = string => {
  const splitter = new GraphemeSplitter();
  return splitter.splitGraphemes(string);
};

const typewriter = new Typewriter(innerdemo, {
  loop: true,
  delay: 45,
  stringSplitter
});

typewriter
  .typeString("Hi, I'm Anas 👋")
  .pauseFor(1000)
  .deleteAll()
  .typeString("I'm a 🚀  developer 🚀")
  .pauseFor(1000)
  .deleteAll()
  .typeString("I ❤️ Happy Hardcore ❤️")
  .pauseFor(1000)
  .deleteAll()
  .start();
