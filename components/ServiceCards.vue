<template>
    <div>
        <div class="mx-auto mt-16 max-w-2xl rounded-3xl shadow-2xl ring-1 ring-gray-200 sm:mt-20 lg:mx-0 lg:flex lg:max-w-none"
            data-aos="fade-up" data-aos-duration="1000">
            <div class="p-8 sm:p-10 lg:flex-auto">
                <h3 class="text-2xl font-bold tracking-tight text-gray-900">{{ title }}</h3>
                <p class="mt-6 text-base leading-7 text-gray-600">{{ description }}</p>
                <div class="mt-10 flex items-center gap-x-4">
                    <h4 class="flex-none text-sm font-semibold leading-6 text-indigo-600">Was ist enthalten</h4>
                    <div class="h-px flex-auto bg-gray-100"></div>
                </div>
                <ul role="list" class="mt-8 grid grid-cols-1 gap-4 text-sm leading-6 text-gray-600 sm:grid-cols-2 sm:gap-6">
                    <li class="flex gap-x-3">
                        <svg class="h-6 w-5 flex-none text-primary" viewBox="0 0 20 20" fill="currentColor"
                            aria-hidden="true">
                            <path fill-rule="evenodd"
                                d="M16.704 4.153a.75.75 0 01.143 1.052l-8 10.5a.75.75 0 01-1.127.075l-4.5-4.5a.75.75 0 011.06-1.06l3.894 3.893 7.48-9.817a.75.75 0 011.05-.143z"
                                clip-rule="evenodd" />
                        </svg>
                        {{ desc1 }}
                    </li>
                    <li class="flex gap-x-3">
                        <svg class="h-6 w-5 flex-none text-primary" viewBox="0 0 20 20" fill="currentColor"
                            aria-hidden="true">
                            <path fill-rule="evenodd"
                                d="M16.704 4.153a.75.75 0 01.143 1.052l-8 10.5a.75.75 0 01-1.127.075l-4.5-4.5a.75.75 0 011.06-1.06l3.894 3.893 7.48-9.817a.75.75 0 011.05-.143z"
                                clip-rule="evenodd" />
                        </svg>
                        {{ desc2 }}

                    </li>
                    <li class="flex gap-x-3">
                        <svg class="h-6 w-5 flex-none text-primary" viewBox="0 0 20 20" fill="currentColor"
                            aria-hidden="true">
                            <path fill-rule="evenodd"
                                d="M16.704 4.153a.75.75 0 01.143 1.052l-8 10.5a.75.75 0 01-1.127.075l-4.5-4.5a.75.75 0 011.06-1.06l3.894 3.893 7.48-9.817a.75.75 0 011.05-.143z"
                                clip-rule="evenodd" />
                        </svg>
                        {{ desc3 }}

                    </li>
                    <li class="flex gap-x-3">
                        <svg class="h-6 w-5 flex-none text-primary" viewBox="0 0 20 20" fill="currentColor"
                            aria-hidden="true">
                            <path fill-rule="evenodd"
                                d="M16.704 4.153a.75.75 0 01.143 1.052l-8 10.5a.75.75 0 01-1.127.075l-4.5-4.5a.75.75 0 011.06-1.06l3.894 3.893 7.48-9.817a.75.75 0 011.05-.143z"
                                clip-rule="evenodd" />
                        </svg>
                        {{ desc4 }}
                    </li>
                </ul>
            </div>
            <div class="-mt-2 p-2 lg:mt-0 lg:w-full lg:max-w-md lg:flex-shrink-0">
                <div
                    class="rounded-2xl bg-gray-100 py-10 text-center ring-1 ring-inset ring-gray-900/5 lg:flex lg:flex-col lg:justify-center lg:py-16">
                    <div class="mx-auto max-w-xs px-8">
                        <p class="text-base font-semibold text-gray-600">{{ heading }}
                        </p>
                        <p class="mt-6 flex items-baseline justify-center gap-x-2">
                            <span class="text-5xl font-bold tracking-tight text-gray-900">{{ payment }}</span>
                            <span class="text-sm font-semibold leading-6 tracking-wide text-gray-600">{{ currency }}</span>
                        </p>
                        <Offer />
                        <p class="mt-6 text-xs leading-5 text-gray-600">Gerne unterbreite ich Ihnen eine
                            unverbindliche Offerte.</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
const probs = defineProps({
    title: String,
    description: String,
    desc1: String,
    desc2: String,
    desc3: String,
    desc4: String,
    heading: String,
    payment: String,
    currency: String,
});
</script>

<style lang="scss" scoped></style>