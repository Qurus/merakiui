<template>
    <view-component :name="name" :code="code">
        <div class="py-6" slot="component">
            <header>
                <nav class="bg-white shadow dark:bg-gray-800">
                    <div class="container px-6 py-3 mx-auto ">
                        <div class="md:flex md:items-center md:justify-between">
                            <div class="flex items-center justify-between">
                                <div class="text-xl font-semibold text-gray-700">
                                    <a class="text-xl font-bold text-gray-800 dark:text-white md:text-2xl hover:text-gray-700 dark:hover:text-gray-300" href="#">Brand</a>
                                </div>

                                <div class="flex md:hidden">
                                    <button @click="isOpen = !isOpen" type="button" class="text-gray-500 dark:text-gray-200 hover:text-gray-600 dark:hover:text-gray-400 focus:outline-none focus:text-gray-600 dark:focus:text-gray-400" aria-label="toggle menu">
                                        <svg viewBox="0 0 24 24" class="w-6 h-6 fill-current">
                                            <path fill-rule="evenodd" d="M4 5h16a1 1 0 0 1 0 2H4a1 1 0 1 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2z"></path>
                                        </svg>
                                    </button>
                                </div>
                            </div>

                            <div :class="!isOpen ? 'hidden' : ''" class="-mx-4 md:flex md:items-center">
                                <a href="#" class="block mx-4 mt-2 text-sm text-gray-700 capitalize md:mt-0 dark:text-gray-200 hover:text-blue-600 dark:hover:text-indigo-400">Web developers</a>
                                <a href="#" class="block mx-4 mt-2 text-sm text-gray-700 capitalize md:mt-0 dark:text-gray-200 hover:text-blue-600 dark:hover:text-indigo-400">Web Designers</a>
                                <a href="#" class="block mx-4 mt-2 text-sm text-gray-700 capitalize md:mt-0 dark:text-gray-200 hover:text-blue-600 dark:hover:text-indigo-400">UI/UX Designers</a>
                                <a href="#" class="block mx-4 mt-2 text-sm text-gray-700 capitalize md:mt-0 dark:text-gray-200 hover:text-blue-600 dark:hover:text-indigo-400">Contact</a>
                            </div>
                        </div>
                    </div>
                </nav>

                <div class="w-full bg-center bg-cover h-128" style="background-image: url(https://images.unsplash.com/photo-1504384308090-c894fdcc538d?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1050&q=80);">
                    <div class="flex items-center justify-center w-full h-full bg-gray-900 bg-opacity-50">
                        <div class="text-center">
                            <h1 class="text-2xl font-semibold text-white uppercase md:text-3xl">Build Your new <span class="text-blue-400 underline">Saas</span></h1>
                            <button class="px-4 py-2 mt-4 text-sm font-medium text-white uppercase transition-colors duration-200 transform bg-blue-600 rounded-md hover:bg-blue-500 focus:outline-none focus:bg-blue-500">Start project</button>
                        </div>
                    </div>
                </div>
            </header>
        </div>
    </view-component>
</template>

<script>
    export default {
        data() {
            return {
                name: 'With Background Image',
                isOpen: false,
                code: `
        <header>
            <nav class="bg-white shadow dark:bg-gray-800">
                <div class="container px-6 py-3 mx-auto ">
                    <div class="md:flex md:items-center md:justify-between">
                        <div class="flex items-center justify-between">
                            <div class="text-xl font-semibold text-gray-700">
                                <a class="text-xl font-bold text-gray-800 dark:text-white md:text-2xl hover:text-gray-700 dark:hover:text-gray-300" href="#">Brand</a>
                            </div>

                            <!-- Mobile menu button -->
                            <div class="flex md:hidden">
                                <button type="button" class="text-gray-500 dark:text-gray-200 hover:text-gray-600 dark:hover:text-gray-400 focus:outline-none focus:text-gray-600 dark:focus:text-gray-400" aria-label="toggle menu">
                                    <svg viewBox="0 0 24 24" class="w-6 h-6 fill-current">
                                        <path fill-rule="evenodd" d="M4 5h16a1 1 0 0 1 0 2H4a1 1 0 1 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2z"></path>
                                    </svg>
                                </button>
                            </div>
                        </div>

                        <!-- Mobile Menu open: "block", Menu closed: "hidden" -->
                        <div class="hidden -mx-4 md:flex md:items-center">
                            <a href="#" class="block mx-4 mt-2 text-sm text-gray-700 capitalize md:mt-0 dark:text-gray-200 hover:text-blue-600 dark:hover:text-indigo-400">Web developers</a>
                            <a href="#" class="block mx-4 mt-2 text-sm text-gray-700 capitalize md:mt-0 dark:text-gray-200 hover:text-blue-600 dark:hover:text-indigo-400">Web Designers</a>
                            <a href="#" class="block mx-4 mt-2 text-sm text-gray-700 capitalize md:mt-0 dark:text-gray-200 hover:text-blue-600 dark:hover:text-indigo-400">UI/UX Designers</a>
                            <a href="#" class="block mx-4 mt-2 text-sm text-gray-700 capitalize md:mt-0 dark:text-gray-200 hover:text-blue-600 dark:hover:text-indigo-400">Contact</a>
                        </div>
                    </div>
                </div>
            </nav>

            <div class="w-full bg-center bg-cover h-128" style="background-image: url(https://images.unsplash.com/photo-1504384308090-c894fdcc538d?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1050&q=80);">
                <div class="flex items-center justify-center w-full h-full bg-gray-900 bg-opacity-50">
                    <div class="text-center">
                        <h1 class="text-2xl font-semibold text-white uppercase md:text-3xl">Build Your new <span class="text-blue-400 underline">Saas</span></h1>
                        <button class="px-4 py-2 mt-4 text-sm font-medium text-white uppercase transition-colors duration-200 transform bg-blue-600 rounded-md hover:bg-blue-500 focus:outline-none focus:bg-blue-500">Start project</button>
                    </div>
                </div>
            </div>
        </header>`,
            }
        }
    }
</script>