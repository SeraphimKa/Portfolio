<script setup lang="ts">

defineProps<({
    techs: string[]
})>()
</script>

<template>
    <section id="tech-stack" class="wrapper">
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
    justify-content: space-around;
    align-items: center;
    width: 80vw;
    margin: 10px;
    background-color: var(--secondary);
    padding: 10px;
}

li {
    list-style: none;
    height: 60px;
    width: 70px;
    background-image: linear-gradient(45deg, #c27829 0%, #a74d2d 25%, #a51e32 50%, #861744 75%, #6b124f 100%);

    flex-grow: 1;
    display: flex;
    align-items: center;
    justify-content: center;
    border-radius: 10px;
    box-shadow: 2px 2px 5px #000;
    transition: all 0.25s;
    cursor: pointer;
}

li:hover {
    background-image: linear-gradient(45deg, #f09433 0%, #e6683c 25%, #dc2743 50%, #cc2366 75%, #bc1888 100%);
    transform: scale(1.05, 1.05);
}

@media screen and (width > 768px) {
    ul {
        gap: 45px;
    }
}
</style>