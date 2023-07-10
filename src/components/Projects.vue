<script setup lang="ts">
defineProps<({
    projects: string[]
})>()
</script>
<template>
    <section id="projects" class="wrapper">
        <h2>PROJECTS</h2>
        <ul>
            <li v-for="project in projects">
                <img :src="project" width="150" height="150">

            </li>
        </ul>
    </section>
</template>

<style scoped>
ul {
    display: flex;
    gap: 15px;
    flex-wrap: wrap;
    justify-content: space-around;
    align-items: center;
    margin: 10px;
    background-color: var(--secondary);
    padding: 10px;
}

li {
    list-style: none;
}
</style>