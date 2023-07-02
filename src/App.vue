<script setup>
//TechStack
import TechStack from './components/TechStack.vue';
import html5 from './assets/html5.svg'
import css from './assets/css.svg'
import javascript from './assets/javascript.svg'
import vue from './assets/vue.svg'
import tailwind from './assets/tailwind.svg'

const techs = [html5, css, javascript, vue, tailwind]

//AboutMe
import AboutMe from './components/AboutMe.vue'

//Projects
import Projects from './components/Projects.vue';
const projects = ['link1', 'link2']
</script>

<template>
  <header>
    <h1>
      Front-End Web Developer 👋🏻
    </h1>
    <div class="flex">
      <img src="" alt="picture">
      <p>Hi, I'm Seraphim Kaniaris, passionate Front-End Developer based in Athens, Greece</p>
    </div>
  </header>

  <TechStack :techs="techs" />

  <AboutMe />

  <Projects :projects="projects" />
</template>

<style>
* {
  color: var(--text);
}

header {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100vh;
}

section {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin:  1rem;
  margin-bottom: 50vh;
  padding: 1px 1px;
}

h1 {
  background: var(--primary);
  padding: 12px;
}

p {
  background-color: var(--secondary);
  padding: 10px;
}

h2 {
  margin: 0;
  white-space: nowrap;
  padding: 10px;
  font-size: 1.5rem;
  background-color: var(--opacity);
  text-decoration-line: underline;
  text-decoration-color: var(--accent);
  text-decoration-thickness: 2px;
}

.flex {
  display: flex;
  gap: 15px;
}
</style>