<script setup lang="ts">
    import { ref } from 'vue'
    import Title from "./components/Title.vue"

    const video = ref(true)
</script>

<template>
    <Title></Title>
    <div @click="() =>  { video = !video }">swap image</div>
    <div v-if="video">
        <video width="320" height="240" controls>
            <source src="./assets/yt.mp4" type="video/mp4">
            doesnt support
        </video>
    </div>
    <div v-else>
        <img 
            src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fs1.zerochan.net%2FShikanoko.Nokonoko.Koshitantan.600.4232336.jpg&f=1&nofb=1&ipt=8c369720bff816882c5650d1fcd087782fa37b34eca5894efee231549e03dc7e"
            alt="whos who shika"
        >
    </div>
</template>

<style scoped>
</style>
