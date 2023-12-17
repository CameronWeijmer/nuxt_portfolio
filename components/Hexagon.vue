<template>
    <div>
        <h1 class="text-2xl font-medium z-10 text-black">{{ title }}</h1>
        <p class="font-light text-sm leading-5 z-10 mt-2 text-black">{{ text }}</p>
    </div>
</template>

<script setup>
const probs = defineProps({
    title: String,
    text: String,
})
</script>

<style lang="scss" scoped></style>