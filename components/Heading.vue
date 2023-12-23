<template>
    <div>
        <div class="bg-white py-24 sm:py-32">
            <div class="mx-auto max-w-7xl px-6 lg:px-8">
                <div class="mx-auto max-w-2xl sm:text-center text-center" data-aos="fade-up" data-aos-duration="1000">
                    <h2 class="text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl">{{ title }}
                    </h2>
                    <p class="mt-6 text-lg leading-8 text-gray-600">{{ text }}</p>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
const probs = defineProps({
    title: String,
    text: String,
})
</script>

<style lang="scss" scoped></style>