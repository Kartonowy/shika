<script setup lang="ts">
    import { ref } from 'vue'
    import Title from "./components/Title.vue"

    const video = ref(true)
</script>

<template>
    <Title></Title>
    <div @click="() =>  { video = !video }">swap</div>
    <div v-if="video">
        <video width="320" height="240" controls>
            <source src="./assets/yt.mp4" type="video/mp4">
            doesnt support
        </video>
    </div>
    <div v-else>
        <img 
            src="https://cdn.discordapp.com/attachments/1275934431009574943/1387891653246849155/koledzy-a-czy-wy-wiecie-ktora-to-prawdziwa-szikanoko-v0-31ggbhyxfb9f1.webp?ex=685efe53&is=685dacd3&hm=3543c64a8a673112f845dca5962011b4a5faf6e76fc7bf63e0886e7df10cba4d&"
            alt="whos who"
        >
    </div>
</template>

<style scoped>
</style>
