<template>
    <div>
        <div id="home" style="background-image: url(/img/background.jpg); background-repeat: none; background-size: cover;"
            class="overflow-hidden relative w-full max-h-full min-h-screen sm:h-full">

            <div class="flex justify-center md:justify-start items-center pt-36 md:pt-0 md:h-screen">
                <div class="text-center md:text-left pl-0 md:pl-32">
                    <div data-aos="fade-up" data-aos-duration="1000">
                        <h1 class="text-white text-6xl font-extrabold font-major">{{ title }}</h1>
                    </div>
                    <div class="pt-5 mx-auto md:mx-0 max-w-lg md:max-w-xl" data-aos="fade-up" data-aos-delay="100"
                        data-aos-duration="1000">
                        <p class="text-primary text-xl">{{ desc1 }} <br class="hidden sm:block" />
                            {{ desc2 }}</p>
                    </div>
                    <div class="pt-5" data-aos="fade-up" data-aos-delay="400" data-aos-duration="1000">
                        <Button :text="buttonTitle" :link="buttonLink" />
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
const probs = defineProps({
    title: String,
    desc1: String,
    desc2: String,
    buttonTitle: String,
    buttonLink: String,
})
</script>

<style scoped></style>