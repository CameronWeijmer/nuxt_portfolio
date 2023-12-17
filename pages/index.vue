<template>
    <div>

        <Landing title="cameron Weijmer" desc1="Vom Konzept zur Website, flink und smart."
            desc2="Melde dich gleich, für einen digitalen Start!" buttonTitle="Meine Projekte" buttonLink="/projekte" />

        <!-- about me -->
        <div id="about" class="overflow-hidden lg:flex-row max-sm:flex-col lg:flex sm:flex-col lg:justify-between sm:justify-between 
        max-sm:justify-center items-center w-full h-full py-10 pb-20 bg-white relative">
            <div class="min-[1349px]:ml-32 lg:mx-auto max-sm:mx-auto max-sm:w-full sm:max-auto sm:w-full  
            w-1/2 text-center items-center flex flex-col">
                <div data-aos="fade-up" data-aos-delay="50" data-aos-duration="1000">
                    <h1 class="text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl">Über mich</h1>
                </div>
                <div class="flex justify-center max-w-sm md:max-w-lg" data-aos="fade-up" data-aos-delay="50"
                    data-aos-duration="1000">
                    <p class=" mt-6 text-lg leading-8 text-gray-600" style="width: 500px;">Mit tiefem Verständnis für die
                        digitale Welt und einer unermüdlichen Wissbegierde strebe ich danach, in jedem Projekt das Beste
                        zu
                        erreichen und innovative Lösungen zu entwickeln.</p>
                </div>
                <div class="flex flex-wrap max-sm:flex-col  items-center justify-center mt-12" style="width: 640px;">
                    <div class=" hexa mx-32 max-sm:mb-48 my-20 flex items-center text-center justify-center relative py-3
                px-2 flex-col" data-aos="fade-up" data-aos-delay="50" data-aos-duration="1000">
                        <div class="absolute bg-white p-3 rounded-full w-14 z-10"
                            style="top: -100px;z-index: 100 !important;border: 1px solid #2161d9">
                            <img src="/img/book.png" class="w-14" alt="">
                        </div>
                        <Hexagon title="Kreativität!"
                            text="Ich nutze meine Kreativität, um Websites zu gestalten, die die Benutzererlebnis verbessern und Ihr Unternehmen hervorheben." />
                    </div>
                    <div class="hexa flex max-sm:mb-48 items-center text-center justify-center py-3 m-2 px-2 relative  flex-col text-white"
                        data-aos="fade-up" data-aos-delay="50" data-aos-duration="1000">
                        <div class="absolute bg-white p-3 rounded-full w-14 z-10"
                            style="top: -100px;z-index: 100 !important;border: 1px solid #2161d9">
                            <img src="/img/book.png" class="w-14" alt="">
                        </div>

                        <Hexagon title="Know-how!"
                            text="Mit tiefem Fachwissen in Programmierung, Datenbanken und Webtechnologien löse ich komplexe IT-Probleme individuell." />
                    </div>
                    <div class="hexa flex m-2 items-center text-center justify-center relative py-3 px-2  flex-col"
                        data-aos="fade-up" data-aos-delay="50" data-aos-duration="1000">
                        <div class="absolute bg-white p-3 rounded-full w-14 z-10"
                            style="top: -100px;z-index: 100 !important;border: 1px solid #2161d9">
                            <img src="/img/book.png" class="w-14" alt="">
                        </div>
                        <Hexagon title="Kundenfokus!"
                            text="Ich arbeite eng mit Kunden zusammen, um sicherzustellen, dass ihre Erwartungen erfüllt werden." />
                    </div>
                </div>
            </div>
            <div class="min-[1349px]:flex sm:hidden max-sm:hidden lg:hidden rounded-l-full overflow-hidden" style="transform: rotate(-60deg) translateX(174px); background: linear-gradient(90deg,#2771ff 0%, #071424 100%);
        width:1500px;height: 390px;">
                <img src="/img/person.png" style="z-index: 100; transform: rotate(60deg); width: 350px;"
                    alt="Cameron Weijmer">
            </div>
        </div>

        <!-- gallery -->

        <div class="mx-auto max-w-2xl sm:text-center text-center pt-28" data-aos="fade-up" data-aos-duration="1000">
            <h2 class="text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl">AI Avatare enthüllt
            </h2>
            <p class="mt-6 text-lg leading-8 text-gray-600">Entdecken Sie meinen ganz persönlichen digitalen
                Doppelgänger.</p>
        </div>
        <div class="py-16 flex justify-evenly items-center mx-auto md:flex-row flex-col flex-wrap">
            <div id="slideshow" class="w-80 md:w-96" data-aos="fade-up" data-aos-delay="50" data-aos-duration="1000">
                <img class="w-full rounded-3xl" src="./assets/gallery/IMG_0112.JPG" alt="" />
                <img class="w-full rounded-3xl" src="./assets/gallery/IMG_0113.JPG" alt="" />
            </div>
            <div id="slideshow2" class="w-80 md:w-96 md:pt-0 pt-10" data-aos="fade-up" data-aos-delay="50"
                data-aos-duration="1000">
                <img class="w-full rounded-3xl" src="./assets/gallery/IMG_0114.JPG" alt="" />
                <img class="w-full rounded-3xl" src="./assets/gallery/IMG_0115.JPG" alt="" />
            </div>
        </div>
    </div>
</template>

<script setup>
definePageMeta({
    layout: "navigation"
})
</script>

<style></style>