<script setup>
//Header
import Header from './components/Header.vue';




//TechStack
import TechStack from './components/TechStack.vue';

const techsRaw = import.meta.glob('./assets/techs/*.svg', { as: 'url', eager: true })
const techs = Object.values(techsRaw)


//AboutMe
import AboutMe from './components/AboutMe.vue'

//Projects
import Projects from './components/Projects.vue';
const projects = ['link1', 'link2']
</script>

<template>
  <Header />

  <TechStack :techs="techs" />

  <AboutMe />

  <Projects :projects="projects" />
</template>

<style>
* {
  color: var(--text);
}

section {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin: 1rem;
  margin-bottom: 50vh;
  padding: 1px 1px;
}

h1 {
  background: var(--primary);
  padding: 12px;
}

p {
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

.wrapper {
  box-shadow: 0 0 20px 0 rgba(0, 0, 0, 0.2);
  padding: 1rem;
  border-radius: 10px;
  background-color: var(--secondary);
}
</style>