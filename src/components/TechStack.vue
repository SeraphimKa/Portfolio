<script setup>
defineProps({
    techs: {
        type: Array,
        required: true
    }
})
</script>

<template>
    <section id="tech-stack">
        <h2>TECH STACK</h2>
        <ul>
            <li v-for="tech in techs"><img :src="tech" width="35"></li>
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