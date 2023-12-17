<template>
    <div>
        <header>
            <nav id="menu-overlay" class="fixed top-0 w-full z-50 duration-700 bg-black">
                <div class="max-w-screen-xl flex flex-wrap items-center justify-between mx-auto p-4">
                    <NuxtLink href="/" class="flex items-center">
                        <img src="./assets/logo.svg" class="h-10 mr-3" alt="Logo Cameron Weijmer" />
                        <span class="self-center text-xl text-white font-semibold whitespace-nowrap">Cameron
                            Weijmer</span>
                    </NuxtLink>
                    <button data-collapse-toggle="navbar-default" type="button"
                        class="inline-flex items-center p-2 w-10 h-10 justify-center text-sm text-white md:hidden hover:opacity-75"
                        aria-controls="navbar-default" aria-expanded="false">
                        <span class="sr-only">Open main menu</span>
                        <svg class="w-5 h-5" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none"
                            viewBox="0 0 17 14">
                            <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                d="M1 1h15M1 7h15M1 13h15" />
                        </svg>
                    </button>
                    <div class="hidden w-full md:block md:w-auto" id="navbar-default">
                        <ul
                            class="font-medium flex flex-col p-4 md:p-0 mt-4 md:flex-row md:space-x-8 md:mt-0 border-white md:border-none">
                            <li>
                                <NuxtLink href="/" class="block py-2 pl-3 pr-4 text-white md:p-0">Home</NuxtLink>
                            </li>
                            <li>
                                <NuxtLink href="/#ueber-mich"
                                    class="block py-2 pl-3 pr-4 text-white hover:text-primary duration-500 md:border-0 md:p-0">
                                    Über
                                    mich</NuxtLink>
                            </li>
                            <li>
                                <NuxtLink href="/service"
                                    class="block py-2 pl-3 pr-4 text-white font-extrabold hover:text-primary duration-500 md:border-0 md:p-0"
                                    aria-current="page">Service</NuxtLink>
                            </li>
                            <li>
                                <NuxtLink href="/projekte"
                                    class="block py-2 pl-3 pr-4 text-white hover:text-primary duration-500 md:border-0 md:p-0">
                                    Projekte</NuxtLink>
                            </li>
                            <li>
                                <NuxtLink href="kontakt"
                                    class="block py-2 pl-3 pr-4 text-white hover:text-primary duration-500 md:border-0 md:p-0">
                                    Kontakt</NuxtLink>
                            </li>
                        </ul>
                    </div>
                </div>
            </nav>
        </header>

        <!-- output page content -->
        <div class="">
            <slot />
        </div>

        <footer class="bg-gray-100 mt-16 pt-16">
            <div class="relative mx-auto max-w-screen-xl px-4 py-16 sm:px-6 lg:px-8 lg:pt-24">
                <div class="absolute end-4 top-4 sm:end-6 sm:top-6 lg:end-8 lg:top-8">
                    <NuxtLink
                        class="animate-bounce inline-block rounded-full bg-black p-2 text-white shadow transition hover:opacity-75 sm:p-3 lg:p-4"
                        href="/">
                        <span class="sr-only">Back to top</span>

                        <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20" fill="currentColor">
                            <path fill-rule="evenodd"
                                d="M14.707 12.707a1 1 0 01-1.414 0L10 9.414l-3.293 3.293a1 1 0 01-1.414-1.414l4-4a1 1 0 011.414 0l4 4a1 1 0 010 1.414z"
                                clip-rule="evenodd" />
                        </svg>
                    </NuxtLink>
                </div>

                <div class="lg:flex lg:items-end lg:justify-between">
                    <div>
                        <div class="flex justify-center text-teal-600 lg:justify-start items-center">
                            <img class="w-30 h-14" src="./assets/logo.svg" alt="Logo" />
                            <NuxtLink href="/">
                                <p class="pl-5 font-bold text-gray-800 text-xl">Cameron Weijmer</p>
                            </NuxtLink>
                        </div>

                    </div>

                    <ul class="mt-12 flex flex-wrap justify-center gap-6 md:gap-8 lg:mt-0 lg:justify-end lg:gap-12">
                        <li>
                            <NuxtLink class="text-gray-700 transition hover:text-gray-700/75" href="/#about">
                                Über mich
                            </NuxtLink>
                        </li>

                        <li>
                            <NuxtLink class="text-gray-700 transition hover:text-gray-700/75" href="/service">
                                Service
                            </NuxtLink>
                        </li>

                        <li>
                            <NuxtLink class="text-gray-700 transition hover:text-gray-700/75" href="/kontakt">
                                Kontakt
                            </NuxtLink>
                        </li>

                        <li>
                            <NuxtLink class="text-gray-700 transition hover:text-gray-700/75" href="/impressum">
                                Impressum
                            </NuxtLink>
                        </li>
                        <li>
                            <NuxtLink class="text-gray-700 transition hover:text-gray-700/75"
                                href="./assets/files/Datenschutzerklärung.pdf" target="_blank">
                                Datenschutz
                            </NuxtLink>
                        </li>
                    </ul>
                </div>

                <p class="mt-12 text-center text-sm text-gray-500 lg:text-right">
                    &copy; 2023 Cameron Weijmer. All rights reserved.
                </p>
            </div>
        </footer>
    </div>
</template>

<style scoped>
.router-link-exact-active {
    color: #ee407b;
}
</style>