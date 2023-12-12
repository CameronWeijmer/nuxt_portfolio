<template>
    <div>
        <header>
            <nav id="menu-overlay" class="fixed top-0 w-full z-50 duration-700 bg-black">
                <div class="max-w-screen-xl flex flex-wrap items-center justify-between mx-auto p-4">
                    <a href="index.html" class="flex items-center">
                        <img src="./assets/logo.svg" class="h-10 mr-3" alt="Logo Cameron Weijmer" />
                        <span class="self-center text-xl text-white font-semibold whitespace-nowrap">Cameron
                            Weijmer</span>
                    </a>
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
                                <a href="index.html" class="block py-2 pl-3 pr-4 text-white md:p-0">Home</a>
                            </li>
                            <li>
                                <a href="index.html#about"
                                    class="block py-2 pl-3 pr-4 text-white hover:text-primary duration-500 md:border-0 md:p-0">Über
                                    mich</a>
                            </li>
                            <li>
                                <a href="service.html"
                                    class="block py-2 pl-3 pr-4 text-white font-extrabold hover:text-primary duration-500 md:border-0 md:p-0"
                                    aria-current="page">Service</a>
                            </li>
                            <li>
                                <a href="projekte.html"
                                    class="block py-2 pl-3 pr-4 text-white hover:text-primary duration-500 md:border-0 md:p-0">Projekte</a>
                            </li>
                            <li>
                                <a href="kontakt.html"
                                    class="block py-2 pl-3 pr-4 text-white hover:text-primary duration-500 md:border-0 md:p-0">Kontakt</a>
                            </li>
                        </ul>
                    </div>
                </div>
            </nav>
        </header>

        <!-- output page content -->
        <div class="container mx-auto p-4">
            <slot />
        </div>
    </div>
</template>

<style scoped>
.router-link-exact-active {
    color: #ee407b;
}
</style>