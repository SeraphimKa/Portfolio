<script setup lang="ts">

</script>

<template>
    <header id="header">
        <div class="wrapper">
            <div class="top-left"></div>
            <h1>
                Front-End Web Developer 👋🏻
            </h1>
            <div class="flex">
                <img src="link" alt="picture">
                <p>Hi, I'm Seraphim Kaniaris, passionate Front-End Developer based in Athens, Greece</p>
            </div>
            <div class="bottom-right"></div>
        </div>
    </header>
</template>

<style scoped>
header {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    height: 100vh;
}

p {
    font-family: serif;
    font-style: italic;
}

.top-left {
    border-top: 15px solid var(--accent);
    border-left: 15px solid var(--accent);
    border-bottom: 15px solid transparent;
    border-right: 15px solid transparent;
    height: 60px;
    width: 60px;
    border-top-left-radius: 10px;
}

.bottom-right {
    float: right;
    border-top: 15px solid transparent;
    border-left: 15px solid transparent;
    border-bottom: 15px solid var(--accent);
    border-right: 15px solid var(--accent);
    height: 60px;
    width: 60px;
    border-bottom-right-radius: 10px;
}
</style>