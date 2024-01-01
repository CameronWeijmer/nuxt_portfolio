<template>
    <div>
        <form class="pt-10" action="https://formspree.io/f/moqbbzbo" method="POST" name="contact-form">
            <div class=" flex flex-row flex-wrap justify-evenly">
                <div class="max-w-md pb-20 md:pb-0" data-aos="fade-up" data-aos-duration="1000">
                    <img class="w-screen" :src="imageSrc" alt="Email illustration" />
                </div>
                <div class="max-w-xs md:max-w-2xl" data-aos="fade-up" data-aos-duration="1000">
                    <div class="flex justify-between">
                        <div class="w-full md:w-1/2 mb-4">
                            <!-- vorname -->
                            <InputLabel labelFor="vorname" labelText="Vorname" star="*" inputType="text" inputId="vorname"
                                inputName="Vorname" inputPlace="Ihr Vorname" />
                        </div>
                        <div class="p-3">
                        </div>
                        <div class="w-full md:w-1/2 mb-4">
                            <InputLabel labelFor="nachname" labelText="Nachname" star="*" inputType="text"
                                inputId="nachname" inputName="Nachname" inputPlace="Ihr Nachname" />
                        </div>
                    </div>
                    <div class="mb-4">
                        <InputLabel labelFor="email" labelText="E-Mail" star="*" inputType="email" inputId="email"
                            inputName="Email" inputPlace="Ihre E-Mail" />
                    </div>
                    <div class="mb-4">
                        <InputLabel labelFor="telefon" labelText="Telefonnummer" star="" inputType="tel" inputId="telefon"
                            inputName="Telefon" inputPlace="Ihre Telefonnummer" />
                    </div>
                    <div class="mb-4">
                        <InputLabel labelFor="firma" labelText="Firma" star="" inputType="text" inputId="firma"
                            inputName="Firma" inputPlace="Ihre Firma" />
                    </div>

                    <div>
                        <label for="message" class="block text-gray-600 font-medium mb-1">Nachricht<span
                                class="text-[#ff0000]">*</span></label>
                        <textarea name="Nachricht" id="message" rows="4" maxlength="350"
                            class="w-full px-3 py-2 border rounded-md outline-none focus:ring-0 focus:border-primary duration-500"
                            placeholder="Ihre Nachricht" required></textarea>

                    </div>

                    <div class="pt-5">
                        <button type="submit" id="btnsubmit" onclick="submitForm()"><a
                                class="relative inline-flex items-center justify-start py-3 pl-4 pr-12 overflow-hidden font-semibold text-indigo-600 transition-all duration-500 ease-in-out rounded hover:pl-10 hover:pr-6 bg-gray-50 group">
                                <span
                                    class="absolute bottom-0 left-0 w-full h-1 transition-all duration-150 ease-in-out bg-primary group-hover:h-full"></span>
                                <span class="absolute right-0 pr-4 duration-200 ease-out group-hover:translate-x-12">
                                    <svg class="w-5 h-5 text-black" fill="none" stroke="currentColor" viewBox="0 0 24 24"
                                        xmlns="http://www.w3.org/2000/svg">
                                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                            d="M14 5l7 7m0 0l-7 7m7-7H3"></path>
                                    </svg>
                                </span>
                                <span
                                    class="absolute left-0 pl-2.5 -translate-x-12 group-hover:translate-x-0 ease-out duration-200">
                                    <svg class="w-5 h-5 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24"
                                        xmlns="http://www.w3.org/2000/svg">
                                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                            d="M14 5l7 7m0 0l-7 7m7-7H3"></path>
                                    </svg>
                                </span>
                                <span class="relative w-full text-left transition-colors 
                                duration-200 ease-in-out group-hover:text-white font">Senden</span>
                            </a></button>
                    </div>
                </div>
            </div>
        </form>
    </div>
</template>

<script setup>
const probs = defineProps({
    imageSrc: String,
})
</script>

<style scoped></style>