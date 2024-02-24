<script setup>
import {Head} from '@inertiajs/vue3';
import {ref} from 'vue';
import Slider from "@/Components/Slider.vue";
import SecondaryButton from "@/Components/SecondaryButton.vue";

const isOpen = ref(false);

</script>

<template>
    <Head title="Zubairi Yahya - Fullstack Developer"/>

    <div class="w-full text-white fixed top-0 left-0 z-50">
        <div class="container mx-auto py-4 px-6 flex justify-end md:justify-center md:items-center">

            <nav
                class="hidden md:flex items-center justify-center space-x-4 w-1/2 h-12 rounded-full bg-gradient-to-r from-teal-400 bg-opacity-50 backdrop-blur-sm">
                <a href="#projects" class="hover:text-teal-400">Project</a>
                <a href="#experience" class="hover:text-teal-400">Work Experience</a>
                <a href="#contact" class="hover:text-teal-400">Contact Me</a>
            </nav>

            <div class="md:hidden">
                <button @click="isOpen = !isOpen" class="text-white focus:outline-none">
                    <svg class="h-6 w-6" fill="none" stroke="currentColor" viewBox="0 0 24 24"
                         xmlns="http://www.w3.org/2000/svg">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                              d="M4 6h16M4 12h16m-7 6h7"></path>
                    </svg>
                </button>
            </div>

            <div v-if="isOpen" @click="isOpen = false"
                 class="md:hidden absolute top-16 right-6 bg-gray-800 mt-2 px-4 py-2 rounded-lg bg-opacity-75">
                <a href="#projects" class="block py-1">Project</a>
                <a href="#experience" class="block py-1">Work Experience</a>
                <a href="#contact" class="block py-1">Contact Me</a>
            </div>
        </div>
    </div>

    <section id="header"
             class="relative sm:flex sm:justify-center sm:items-center min-h-screen bg-dots-darker bg-center bg-gray-100 dark:bg-dots-lighter dark:bg-gray-900 selection:bg-red-500 selection:text-white">
        <div class="max-w-7xl mx-auto p-6 lg:p-8">
            <div class="mt-24 md:mt-0">
                <p class="text-lg font-mono text-gray-900 dark:text-teal-500">Hi, my name is</p>
                <p class="mt-4 md:mt-4 text-6xl md:text-8xl font-semibold text-gray-900 dark:text-white">Zubairi Yahya</p>
                <p class="mt-8 md:mt-4 text-5xl font-semibold text-gray-900 dark:text-gray-400">I develop things for web and
                    mobile</p>

                <p class="mt-8 md:mt-4 text-gray-500 dark:text-gray-400 text-lg leading-relaxed">
                    I'm a software engineer with over three years of experience in developing applications using PHP,
                    JavaScript, Laravel, and Vue.js. I also have expertise in mobile app development with Kotlin and
                    Flutter. Programmer at <span class="text-teal-500"> Bappelitbang Kab.Tapin </span>
                </p>
            </div>
        </div>
    </section>

    <div class="bg-gradient-to-r from-teal-400 to-blue-400">
        <br>
    </div>

    <section id="projects"
             class="relative sm:flex sm:justify-center sm:items-center min-h-screen bg-dots-darker bg-center bg-gray-100 dark:bg-dots-lighter dark:bg-gray-900 selection:bg-red-500 selection:text-white">
        <div class="max-w-7xl mx-auto p-6 lg:p-8">
            <div class="flex justify-center text-justify md:text-center">
                <div>
                    <p class="mt-6 md:mt-16 text-4xl md:text-5xl font-semibold text-gray-900 dark:text-white">🚀 Recent Projects</p>
                    <p class="mt-6 text-xl w-full md:px-60 font-semibold text-gray-900 dark:text-gray-300">
                        Working of variety of projects, from small to full-scale application, also developed a wide
                        array of features and functionalities in projects
                    </p>
                </div>
            </div>

            <div class="mt-16">
                <div class="grid grid-cols-1 gap-6 lg:gap-8">

                    <a href="https://e-sppd.bappelitbang.tapinkab.go.id/"
                       class="scale-100 p-6 bg-white dark:bg-gray-800/50 dark:bg-gradient-to-bl from-gray-700/50 via-transparent dark:ring-1 dark:ring-inset dark:ring-white/5 rounded-lg shadow-2xl shadow-gray-500/20 dark:shadow-none flex motion-safe:hover:scale-[1.01] transition-all duration-250 focus:outline focus:outline-2 focus:outline-red-500">
                        <div class="overflow-x-clip">
                            <div
                                class="h-16 w-16 bg-white-50 dark:bg-white flex items-center justify-center rounded-full">
                                <img width="50"
                                     src="https://e-sppd.bappelitbang.tapinkab.go.id/build/assets/e-sppd-acfc3936.png"
                                     alt="logo">
                            </div>

                            <h2 class="mt-4 text-2xl font-semibold text-gray-900 dark:text-white">Electronic Official
                                Travel Document</h2>
                            <h2 class="text-lg font-semibold text-gray-900 dark:text-teal-300">Fullstack Developer</h2>

                            <p class="mt-4 mb-6 text-gray-500 dark:text-gray-400 text-md text-justify leading-relaxed">
                                Solution offers a modern approach to managing official travel documents
                                electronically. Users can effortlessly create, send, and track travel documents with
                                efficiency. Features such as document template creation, automated approval processes,
                                and real-time tracking ensure effectiveness and speed in managing official travel
                                documents. Designed to enhance productivity and reduce administrative costs in travel
                                document management, our application streamlines the entire process, providing a
                                seamless experience for users.
                            </p>

                            <Slider :images="[
                                '@/../../img/e-sppd-login.png',
                                '@/../../img/e-sppd-dashboard.png',
                                '@/../../img/e-sppd-dashboard-2.png',
                            ]"/>

                        </div>

                        <svg
                            xmlns="http://www.w3.org/2000/svg"
                            fill="none"
                            viewBox="0 0 24 24"
                            stroke-width="1.5"
                            class="hidden md:block self-center shrink-0 stroke-red-500 w-6 h-6 mx-6"
                        >
                            <path
                                stroke-linecap="round"
                                stroke-linejoin="round"
                                d="M4.5 12h15m0 0l-6.75-6.75M19.5 12l-6.75 6.75"
                            />
                        </svg>
                    </a>

                    <a href="https://e-monev.bappelitbang.tapinkab.go.id/"
                       class="scale-100 p-6 bg-white dark:bg-gray-800/50 dark:bg-gradient-to-bl from-gray-700/50 via-transparent dark:ring-1 dark:ring-inset dark:ring-white/5 rounded-lg shadow-2xl shadow-gray-500/20 dark:shadow-none flex motion-safe:hover:scale-[1.01] transition-all duration-250 focus:outline focus:outline-2 focus:outline-red-500">
                        <div class="overflow-x-clip">

                            <h2 class="mt-4 text-2xl font-semibold text-gray-900 dark:text-white">Electronic Monitoring
                                & Evaluation</h2>

                            <h2 class="text-lg font-semibold text-gray-900 dark:text-teal-300">Front End Developer</h2>

                            <p class="mt-4 mb-6 text-gray-500 dark:text-gray-400 text-md text-justify leading-relaxed">
                                Electronic monitoring and evaluation application is designed to facilitate the
                                monitoring and evaluation of local government performance against predetermined targets.
                                By integrating key documents such as work plans, strategic plans, and medium-term
                                development plans at the local level, our application provides a comprehensive platform
                                for managing and assessing the implementation of programs and projects
                            </p>

                            <Slider :images="[
                                '@/../../img/e-monev-login.png',
                                '@/../../img/e-monev-visi.png',
                                '@/../../img/e-monev-renstra.png',
                            ]"/>

                        </div>

                        <svg
                            xmlns="http://www.w3.org/2000/svg"
                            fill="none"
                            viewBox="0 0 24 24"
                            stroke-width="1.5"
                            class="hidden md:block self-center shrink-0 stroke-red-500 w-6 h-6 mx-6"
                        >
                            <path
                                stroke-linecap="round"
                                stroke-linejoin="round"
                                d="M4.5 12h15m0 0l-6.75-6.75M19.5 12l-6.75 6.75"
                            />
                        </svg>
                    </a>

                    <div
                        class="scale-100 p-6 bg-white dark:bg-gray-800/50 dark:bg-gradient-to-bl from-gray-700/50 via-transparent dark:ring-1 dark:ring-inset dark:ring-white/5 rounded-lg shadow-2xl shadow-gray-500/20 dark:shadow-none flex motion-safe:hover:scale-[1.01] transition-all duration-250 focus:outline focus:outline-2 focus:outline-red-500">
                        <div class="overflow-x-clip">
                            <h2 class="mt-4 text-2xl font-semibold text-gray-900 dark:text-white">Cardia Watch</h2>

                            <h2 class="text-lg font-semibold text-gray-900 dark:text-teal-300">Fullstack Developer</h2>

                            <p class="mt-4 mb-6 text-gray-500 dark:text-gray-400 text-md text-justify leading-relaxed">
                                This application offers an innovative solution for real-time monitoring and tracking of
                                patient health using smartwatches. Developed as a mobile application, the platform
                                enables patients to receive early detection of health conditions and provides accurate
                                progress records while they engage in activities anywhere. With advanced features such
                                as heart rate monitoring, activity tracking, and other health parameters, the
                                application assists patients and healthcare providers in effectively monitoring patient
                                health conditions. Thus, the application aims to enhance the quality of life for
                                patients and provide more responsive and personalized healthcare services
                            </p>

                            <Slider :images="[
                                '@/../../img/cardia-home.png',
                                '@/../../img/cardia-health.png',
                                '@/../../img/cardia-connect.png',
                            ]"/>

                        </div>

                        <svg
                            xmlns="http://www.w3.org/2000/svg"
                            fill="none"
                            viewBox="0 0 24 24"
                            stroke-width="1.5"
                            class="hidden md:block self-center shrink-0 stroke-red-500 w-6 h-6 mx-6"
                        >
                            <path
                                stroke-linecap="round"
                                stroke-linejoin="round"
                                d="M4.5 12h15m0 0l-6.75-6.75M19.5 12l-6.75 6.75"
                            />
                        </svg>
                    </div>

                </div>
            </div>
        </div>
    </section>

    <section id="experience"
             class="relative sm:flex sm:justify-center sm:items-center min-h-screen bg-dots-darker bg-center bg-gray-100 dark:bg-dots-lighter dark:bg-gray-900 selection:bg-red-500 selection:text-white">
        <div class="max-w-7xl mx-auto p-6 lg:p-8">
            <div class="flex justify-center text-justify md:text-center">
                <div>
                    <p class="mt-6 md:mt-16 text-4xl md:text-5xl font-semibold text-gray-900 dark:text-white">💼 Work Experience</p>
                    <p class="mt-6 text-xl w-full md:px-60 font-semibold text-gray-900 dark:text-gray-300">
                        I have previously worked on freelance web and mobile application development projects as a
                        full-stack developer, and held
                        a full-time job as a full-stack developer.
                    </p>
                </div>
            </div>

            <div class="mt-16 mb-10">
                <div class="grid grid-cols-1 gap-6 lg:gap-8">
                    <div
                        class="scale-100 p-14 bg-white dark:bg-gray-800/50 dark:bg-gradient-to-bl from-gray-700/50 via-transparent dark:ring-1 dark:ring-inset dark:ring-white/5 rounded-lg shadow-2xl shadow-gray-500/20 dark:shadow-none flex motion-safe:hover:scale-[1.01] transition-all duration-250 focus:outline focus:outline-2 focus:outline-red-500">
                        <div class="overflow-x-clip">
                            <div class="md:flex justify-between">
                                <div>
                                    <h2 class="mt-4 text-3xl font-semibold text-gray-900 dark:text-white">Bappelitbang
                                        Kabupaten Tapin</h2>
                                    <SecondaryButton class="block sm:hidden mt-4 h-12" disable>Programmer</SecondaryButton>
                                    <p class="mt-6 font-bold text-teal-300 text-lg">June 2022 - Present</p>

                                    <p class="mt-4 mb-6 text-gray-500 dark:text-white text-xl text-justify leading-relaxed">
                                        Working on the core web and mobile experience team that focusing on developer
                                        experience,
                                        design
                                        system, and web performance.
                                    </p>

                                    <p class="mt-6 font-extrabold text-white text-xl">Responsibilities and things I did</p>

                                    <p class="mt-4 mb-6 text-gray-500 dark:text-teal-200 text-xl text-justify leading-relaxed">
                                        - Lead or contribute to technical design, implementation, deployment, and
                                        operational excellence efforts to build and run scalable solutions for complex
                                        engineering challenges.
                                    </p>

                                    <p class="mt-4 mb-6 text-gray-500 dark:text-teal-200 text-xl text-justify leading-relaxed">
                                        - Collaborating with local government teams to develop applications
                                        for regional development
                                    </p>
                                </div>
                                <SecondaryButton class="hidden sm:block h-12" disable>Programmer</SecondaryButton>
                            </div>
                        </div>
                    </div>

                </div>
            </div>
        </div>
    </section>

    <div class="bg-gradient-to-l from-teal-400 to-blue-400">
        <br>
    </div>

    <section id="contact"
             class="relative sm:flex sm:justify-center sm:items-center min-h-screen bg-dots-darker bg-center bg-gray-100 dark:bg-dots-lighter dark:bg-gray-900 selection:bg-red-500 selection:text-white">
        <div class="max-w-7xl mx-auto p-6 lg:p-8">
            <div class="mt-16 md:mt-4">
                <p class="mt-8 text-5xl md:text-6xl font-semibold text-gray-900 dark:text-white">Let's get in touch</p>
                <p class="mt-8 text-6xl md:text-8xl font-semibold text-gray-900 dark:text-gray-400">Have any project ideas?</p>
                <p class="mt-8 text-6xl md:text-8xl font-semibold text-gray-900 dark:text-gray-400">Have any question?</p>

                <div class="md:w-1/2 flex items-center mt-24">
                    <div
                        class="h-24 md:h-32 w-24 md:w-32 bg-white-50 dark:bg-white flex items-center justify-center rounded-full overflow-hidden">
                        <img width="200"
                             src="/../img/profile.jpg"
                             alt="logo">
                    </div>
                    <div class="ml-6 text-xl text-white">
                        <p class="text-teal-500 mb-6">Contact me via</p>
                        <p>
                            📧 zubairiyhy22@gmail.com
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </section>

</template>

<style>
.bg-dots-darker {
    background-image: url("data:image/svg+xml,%3Csvg width='30' height='30' viewBox='0 0 30 30' fill='none' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M1.22676 0C1.91374 0 2.45351 0.539773 2.45351 1.22676C2.45351 1.91374 1.91374 2.45351 1.22676 2.45351C0.539773 2.45351 0 1.91374 0 1.22676C0 0.539773 0.539773 0 1.22676 0Z' fill='rgba(0,0,0,0.07)'/%3E%3C/svg%3E");
}

@media (prefers-color-scheme: dark) {
    .dark\:bg-dots-lighter {
        background-image: url("data:image/svg+xml,%3Csvg width='30' height='30' viewBox='0 0 30 30' fill='none' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M1.22676 0C1.91374 0 2.45351 0.539773 2.45351 1.22676C2.45351 1.91374 1.91374 2.45351 1.22676 2.45351C0.539773 2.45351 0 1.91374 0 1.22676C0 0.539773 0.539773 0 1.22676 0Z' fill='rgba(255,255,255,0.07)'/%3E%3C/svg%3E");
    }
}
</style>
