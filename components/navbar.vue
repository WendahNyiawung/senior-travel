<template>
    <div>
        <nav class="bg-white dark:bg-gray-800 shadow">
        <div class="container mx-auto px-6 py-2">
            <div class="flex flex-col md:flex-row md:justify-between md:items-center">
                <div class="flex justify-between items-center">
                    <div class="flex items-center">
                        <nuxt-link to="/">
                         <img src="../assets/img/flight.png" alt="" class="h-20">
                        </nuxt-link>

                    </div>

                    <!-- Mobile menu button -->
                    <div class="flex md:hidden">
                        <button type="button" class="text-gray-500 dark:text-gray-200 hover:text-gray-600 dark:hover:text-gray-400 focus:outline-none focus:text-gray-600 dark:focus:text-gray-400" aria-label="toggle menu">
                            <svg viewBox="0 0 24 24" class="h-6 w-6 fill-current">
                                <path fill-rule="evenodd" d="M4 5h16a1 1 0 0 1 0 2H4a1 1 0 1 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2z"></path>
                            </svg>
                        </button>
                    </div>
                </div>

                <!-- Mobile Menu open: "block", Menu closed: "hidden" -->
                <div class="md:flex items-center">

                    <div class="flex items-center py-2 -mx-1 md:mx-0">
                        <nuxt-link to="/login"  class="block w-1/2 px-3 py-2 mx-1 rounded text-center text-sm bg-gray-500 font-medium text-white leading-5 hover:bg-green-600 md:mx-2 md:w-auto">Login</nuxt-link>
                        <nuxt-link to="/signup" class="block w-1/2 px-3 py-2 mx-1 rounded text-center text-sm bg-green-400 font-medium text-white leading-5 hover:bg-green-600 md:mx-0 md:w-auto">Join for Free</nuxt-link>
                    </div>

                </div>
            </div>

        </div>
    </nav>
    </div>
</template>