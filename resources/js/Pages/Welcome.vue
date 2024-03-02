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
            <div class="mt-24 md:mt-0" data-aos="fade-right">
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
                <div data-aos="fade-right"
                     data-aos-offset="300"
                     data-aos-easing="ease-in-sine">
                    <p class="mt-6 md:mt-16 text-4xl md:text-5xl font-semibold text-gray-900 dark:text-white">🚀 Recent Projects</p>
                    <p class="mt-6 text-xl w-full md:px-60 font-semibold text-gray-900 dark:text-gray-300">
                        Working of variety of projects, from small to full-scale application, also developed a wide
                        array of features and functionalities in projects
                    </p>
                </div>
            </div>

            <div class="mt-16 mb-16">
                <div class="grid grid-cols-1 gap-6 lg:gap-8">

                    <div data-aos="flip-right">
                        <a href="https://e-sppd.bappelitbang.tapinkab.go.id/"
                           class="scale-100 p-6 bg-white dark:bg-gray-800/50 dark:bg-gradient-to-bl from-gray-700/50 via-transparent dark:ring-1 dark:ring-inset dark:ring-white/5 rounded-lg shadow-2xl shadow-gray-500/20 dark:shadow-none flex motion-safe:hover:scale-[1.01] transition-all duration-250 focus:outline focus:outline-2 focus:outline-red-500">
                            <div class="overflow-x-clip">
                                <div
                                    class="h-16 w-16 bg-white-50 dark:bg-white flex items-center justify-center rounded-full">
                                    <img width="50"
                                         src="/../img/e-sppd.png"
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

                                <br>

                                <div
                                    class="md:w-1/3 p-6 md:ml-2 bg-white dark:bg-gray-700/50 dark:bg-gradient-to-bl from-gray-700/50 via-transparent dark:ring-1 dark:ring-inset dark:ring-white/5 rounded-lg shadow-2xl shadow-gray-500/20 dark:shadow-none flex motion-safe:hover:scale-[1.01] transition-all duration-250">
                                    <div class="overflow-x-clip">
                                        <h2 class="text-2xl font-semibold text-gray-900 dark:text-white">Featured
                                            technologies used</h2>

                                        <div class="flex">
                                            <svg
                                                viewBox="0 0 62 65"
                                                fill="none"
                                                xmlns="http://www.w3.org/2000/svg"
                                                class="h-16 mt-4 w-auto"
                                            >
                                                <path
                                                    d="M61.8548 14.6253C61.8778 14.7102 61.8895 14.7978 61.8897 14.8858V28.5615C61.8898 28.737 61.8434 28.9095 61.7554 29.0614C61.6675 29.2132 61.5409 29.3392 61.3887 29.4265L49.9104 36.0351V49.1337C49.9104 49.4902 49.7209 49.8192 49.4118 49.9987L25.4519 63.7916C25.3971 63.8227 25.3372 63.8427 25.2774 63.8639C25.255 63.8714 25.2338 63.8851 25.2101 63.8913C25.0426 63.9354 24.8666 63.9354 24.6991 63.8913C24.6716 63.8838 24.6467 63.8689 24.6205 63.8589C24.5657 63.8389 24.5084 63.8215 24.456 63.7916L0.501061 49.9987C0.348882 49.9113 0.222437 49.7853 0.134469 49.6334C0.0465019 49.4816 0.000120578 49.3092 0 49.1337L0 8.10652C0 8.01678 0.0124642 7.92953 0.0348998 7.84477C0.0423783 7.8161 0.0598282 7.78993 0.0697995 7.76126C0.0884958 7.70891 0.105946 7.65531 0.133367 7.6067C0.152063 7.5743 0.179485 7.54812 0.20192 7.51821C0.230588 7.47832 0.256763 7.43719 0.290416 7.40229C0.319084 7.37362 0.356476 7.35243 0.388883 7.32751C0.425029 7.29759 0.457436 7.26518 0.498568 7.2415L12.4779 0.345059C12.6296 0.257786 12.8015 0.211853 12.9765 0.211853C13.1515 0.211853 13.3234 0.257786 13.475 0.345059L25.4531 7.2415H25.4556C25.4955 7.26643 25.5292 7.29759 25.5653 7.32626C25.5977 7.35119 25.6339 7.37362 25.6625 7.40104C25.6974 7.43719 25.7224 7.47832 25.7523 7.51821C25.7735 7.54812 25.8021 7.5743 25.8196 7.6067C25.8483 7.65656 25.8645 7.70891 25.8844 7.76126C25.8944 7.78993 25.9118 7.8161 25.9193 7.84602C25.9423 7.93096 25.954 8.01853 25.9542 8.10652V33.7317L35.9355 27.9844V14.8846C35.9355 14.7973 35.948 14.7088 35.9704 14.6253C35.9792 14.5954 35.9954 14.5692 36.0053 14.5405C36.0253 14.4882 36.0427 14.4346 36.0702 14.386C36.0888 14.3536 36.1163 14.3274 36.1375 14.2975C36.1674 14.2576 36.1923 14.2165 36.2272 14.1816C36.2559 14.1529 36.292 14.1317 36.3244 14.1068C36.3618 14.0769 36.3942 14.0445 36.4341 14.0208L48.4147 7.12434C48.5663 7.03694 48.7383 6.99094 48.9133 6.99094C49.0883 6.99094 49.2602 7.03694 49.4118 7.12434L61.3899 14.0208C61.4323 14.0457 61.4647 14.0769 61.5021 14.1055C61.5333 14.1305 61.5694 14.1529 61.5981 14.1803C61.633 14.2165 61.6579 14.2576 61.6878 14.2975C61.7103 14.3274 61.7377 14.3536 61.7551 14.386C61.7838 14.4346 61.8 14.4882 61.8199 14.5405C61.8312 14.5692 61.8474 14.5954 61.8548 14.6253ZM59.893 27.9844V16.6121L55.7013 19.0252L49.9104 22.3593V33.7317L59.8942 27.9844H59.893ZM47.9149 48.5566V37.1768L42.2187 40.4299L25.953 49.7133V61.2003L47.9149 48.5566ZM1.99677 9.83281V48.5566L23.9562 61.199V49.7145L12.4841 43.2219L12.4804 43.2194L12.4754 43.2169C12.4368 43.1945 12.4044 43.1621 12.3682 43.1347C12.3371 43.1097 12.3009 43.0898 12.2735 43.0624L12.271 43.0586C12.2386 43.0275 12.2162 42.9888 12.1887 42.9539C12.1638 42.9203 12.1339 42.8916 12.114 42.8567L12.1127 42.853C12.0903 42.8156 12.0766 42.7707 12.0604 42.7283C12.0442 42.6909 12.023 42.656 12.013 42.6161C12.0005 42.5688 11.998 42.5177 11.9931 42.4691C11.9881 42.4317 11.9781 42.3943 11.9781 42.3569V15.5801L6.18848 12.2446L1.99677 9.83281ZM12.9777 2.36177L2.99764 8.10652L12.9752 13.8513L22.9541 8.10527L12.9752 2.36177H12.9777ZM18.1678 38.2138L23.9574 34.8809V9.83281L19.7657 12.2459L13.9749 15.5801V40.6281L18.1678 38.2138ZM48.9133 9.14105L38.9344 14.8858L48.9133 20.6305L58.8909 14.8846L48.9133 9.14105ZM47.9149 22.3593L42.124 19.0252L37.9323 16.6121V27.9844L43.7219 31.3174L47.9149 33.7317V22.3593ZM24.9533 47.987L39.59 39.631L46.9065 35.4555L36.9352 29.7145L25.4544 36.3242L14.9907 42.3482L24.9533 47.987Z"
                                                    fill="#FF2D20"
                                                />
                                            </svg>

                                            <svg
                                                viewBox="0 0 101 102"
                                                fill="none"
                                                xmlns="http://www.w3.org/2000/svg"
                                                class="h-24 w-auto"
                                            >
                                                <g clip-path="url(#clip0_191_497)">
                                                    <path
                                                        d="M58.4649 21.1224L50.4976 34.9222L42.5306 21.1224H15.9987L50.4979 80.8774L84.9971 21.1224H58.4649Z"
                                                        fill="#41B883"></path>
                                                    <path
                                                        d="M58.4649 21.1224L50.4976 34.9222L42.5306 21.1224H29.7984L50.4979 56.9747L71.1974 21.1224H58.4649Z"
                                                        fill="#34495E"></path>
                                                </g>
                                                <defs>
                                                    <clipPath id="clip0_191_497">
                                                        <rect width="69" height="59.7555" fill="white"
                                                              transform="translate(16 21.1222)"></rect>
                                                    </clipPath>
                                                </defs>
                                            </svg>
                                        </div>
                                    </div>
                                </div>

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
                    </div>

                    <div data-aos="flip-right">
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

                                <br>

                                <div
                                    class="md:w-1/3 p-6 md:ml-2 bg-white dark:bg-gray-700/50 dark:bg-gradient-to-bl from-gray-700/50 via-transparent dark:ring-1 dark:ring-inset dark:ring-white/5 rounded-lg shadow-2xl shadow-gray-500/20 dark:shadow-none flex motion-safe:hover:scale-[1.01] transition-all duration-250">
                                    <div class="overflow-x-clip">
                                        <h2 class="text-2xl font-semibold text-gray-900 dark:text-white">Featured
                                            technologies used</h2>

                                        <div class="flex">
                                            <svg
                                                viewBox="0 0 62 65"
                                                fill="none"
                                                xmlns="http://www.w3.org/2000/svg"
                                                class="h-16 mt-4 w-auto"
                                            >
                                                <path
                                                    d="M61.8548 14.6253C61.8778 14.7102 61.8895 14.7978 61.8897 14.8858V28.5615C61.8898 28.737 61.8434 28.9095 61.7554 29.0614C61.6675 29.2132 61.5409 29.3392 61.3887 29.4265L49.9104 36.0351V49.1337C49.9104 49.4902 49.7209 49.8192 49.4118 49.9987L25.4519 63.7916C25.3971 63.8227 25.3372 63.8427 25.2774 63.8639C25.255 63.8714 25.2338 63.8851 25.2101 63.8913C25.0426 63.9354 24.8666 63.9354 24.6991 63.8913C24.6716 63.8838 24.6467 63.8689 24.6205 63.8589C24.5657 63.8389 24.5084 63.8215 24.456 63.7916L0.501061 49.9987C0.348882 49.9113 0.222437 49.7853 0.134469 49.6334C0.0465019 49.4816 0.000120578 49.3092 0 49.1337L0 8.10652C0 8.01678 0.0124642 7.92953 0.0348998 7.84477C0.0423783 7.8161 0.0598282 7.78993 0.0697995 7.76126C0.0884958 7.70891 0.105946 7.65531 0.133367 7.6067C0.152063 7.5743 0.179485 7.54812 0.20192 7.51821C0.230588 7.47832 0.256763 7.43719 0.290416 7.40229C0.319084 7.37362 0.356476 7.35243 0.388883 7.32751C0.425029 7.29759 0.457436 7.26518 0.498568 7.2415L12.4779 0.345059C12.6296 0.257786 12.8015 0.211853 12.9765 0.211853C13.1515 0.211853 13.3234 0.257786 13.475 0.345059L25.4531 7.2415H25.4556C25.4955 7.26643 25.5292 7.29759 25.5653 7.32626C25.5977 7.35119 25.6339 7.37362 25.6625 7.40104C25.6974 7.43719 25.7224 7.47832 25.7523 7.51821C25.7735 7.54812 25.8021 7.5743 25.8196 7.6067C25.8483 7.65656 25.8645 7.70891 25.8844 7.76126C25.8944 7.78993 25.9118 7.8161 25.9193 7.84602C25.9423 7.93096 25.954 8.01853 25.9542 8.10652V33.7317L35.9355 27.9844V14.8846C35.9355 14.7973 35.948 14.7088 35.9704 14.6253C35.9792 14.5954 35.9954 14.5692 36.0053 14.5405C36.0253 14.4882 36.0427 14.4346 36.0702 14.386C36.0888 14.3536 36.1163 14.3274 36.1375 14.2975C36.1674 14.2576 36.1923 14.2165 36.2272 14.1816C36.2559 14.1529 36.292 14.1317 36.3244 14.1068C36.3618 14.0769 36.3942 14.0445 36.4341 14.0208L48.4147 7.12434C48.5663 7.03694 48.7383 6.99094 48.9133 6.99094C49.0883 6.99094 49.2602 7.03694 49.4118 7.12434L61.3899 14.0208C61.4323 14.0457 61.4647 14.0769 61.5021 14.1055C61.5333 14.1305 61.5694 14.1529 61.5981 14.1803C61.633 14.2165 61.6579 14.2576 61.6878 14.2975C61.7103 14.3274 61.7377 14.3536 61.7551 14.386C61.7838 14.4346 61.8 14.4882 61.8199 14.5405C61.8312 14.5692 61.8474 14.5954 61.8548 14.6253ZM59.893 27.9844V16.6121L55.7013 19.0252L49.9104 22.3593V33.7317L59.8942 27.9844H59.893ZM47.9149 48.5566V37.1768L42.2187 40.4299L25.953 49.7133V61.2003L47.9149 48.5566ZM1.99677 9.83281V48.5566L23.9562 61.199V49.7145L12.4841 43.2219L12.4804 43.2194L12.4754 43.2169C12.4368 43.1945 12.4044 43.1621 12.3682 43.1347C12.3371 43.1097 12.3009 43.0898 12.2735 43.0624L12.271 43.0586C12.2386 43.0275 12.2162 42.9888 12.1887 42.9539C12.1638 42.9203 12.1339 42.8916 12.114 42.8567L12.1127 42.853C12.0903 42.8156 12.0766 42.7707 12.0604 42.7283C12.0442 42.6909 12.023 42.656 12.013 42.6161C12.0005 42.5688 11.998 42.5177 11.9931 42.4691C11.9881 42.4317 11.9781 42.3943 11.9781 42.3569V15.5801L6.18848 12.2446L1.99677 9.83281ZM12.9777 2.36177L2.99764 8.10652L12.9752 13.8513L22.9541 8.10527L12.9752 2.36177H12.9777ZM18.1678 38.2138L23.9574 34.8809V9.83281L19.7657 12.2459L13.9749 15.5801V40.6281L18.1678 38.2138ZM48.9133 9.14105L38.9344 14.8858L48.9133 20.6305L58.8909 14.8846L48.9133 9.14105ZM47.9149 22.3593L42.124 19.0252L37.9323 16.6121V27.9844L43.7219 31.3174L47.9149 33.7317V22.3593ZM24.9533 47.987L39.59 39.631L46.9065 35.4555L36.9352 29.7145L25.4544 36.3242L14.9907 42.3482L24.9533 47.987Z"
                                                    fill="#FF2D20"
                                                />
                                            </svg>

                                            <svg xmlns="http://www.w3.org/2000/svg" height="90" width="100">
                                                <g transform="matrix(.945094 0 0 .945094 6.301403 4.347014)">
                                                    <path
                                                        d="M20.44 13.78c-5.283 7.733-4.625 17.793-.6 26l.296.585.2.37c.037.072.08.143.118.213.07.13.14.255.2.383l.385.673.22.37.447.712.2.3c.2.32.426.638.648.952.005.008.012.017.018.025.035.05.074.1.1.15.192.27.4.536.6.8l.222.288.545.682.208.254a31.65 31.65 0 0 0 .76.884l.016.016c.01.013.02.02.03.033a23.73 23.73 0 0 0 .772.83l.248.254.617.616.252.244a34.49 34.49 0 0 0 .845.783l.16.14.767.66.318.258.64.5.342.265.978.715c.025.017.047.035.072.052.23.16.463.315.697.47l.302.205 1.092.68.302.173.82.468c.15.082.303.16.453.238l.586.3.135.066.24.118.93.438.197.1a32.93 32.93 0 0 0 1.084.459l.264.106 1.023.386.128.046a34.62 34.62 0 0 0 1.14.38l.275.084c.4.12.775.263 1.177.34C67.457 62.6 74.88 42.218 74.88 42.218c-6.233 8.27-17.296 10.45-27.778 8.023-.397-.1-.782-.217-1.17-.334l-.292-.1c-.378-.118-.754-.243-1.126-.373l-.155-.057a35.02 35.02 0 0 1-.993-.375l-.28-.112a31.57 31.57 0 0 1-1.072-.454l-.214-.096-.904-.43-.26-.128a30.9 30.9 0 0 1-.7-.363l-.467-.25a26.89 26.89 0 0 1-.838-.479l-.283-.16c-.368-.22-.732-.45-1.092-.68-.1-.065-.196-.134-.295-.2l-.777-.526-.25-.18-.735-.54-.326-.25-.663-.528-.296-.24-.825-.7c-.028-.025-.06-.05-.1-.077-.294-.263-.583-.533-.868-.804l-.244-.24-.624-.622-.244-.25a31.33 31.33 0 0 1-.765-.824c-.012-.014-.026-.027-.038-.04a31.49 31.49 0 0 1-.776-.9l-.203-.246-.56-.703-.205-.26-.645-.875c-5.82-8.085-7.9-19.235-3.26-28.393M36.84 7.264c-3.82 5.6-3.613 13.094-.633 19.016a24.87 24.87 0 0 0 1.69 2.873c.572.835 1.207 1.83 1.967 2.5.275.3.563.6.857.906.074.077.15.15.226.227a25.21 25.21 0 0 0 .876.829c.012.01.023.022.036.032a26.31 26.31 0 0 0 1.031.87l.232.184a25.13 25.13 0 0 0 1.07.796.6.6 0 0 0 .03.023c.16.113.325.22.488.328.078.052.152.107.23.156a21.65 21.65 0 0 0 .793.495l.112.066.7.4c.082.047.166.088.25.132l.5.258c.025.013.05.023.074.035.337.17.676.33 1.023.485.074.033.15.063.226.095.277.12.557.236.84.347l.36.134a26.33 26.33 0 0 0 .77.273l.348.113c.367.117.73.263 1.113.328 19.725 3.328 24.28-12.14 24.28-12.14-4.105 6.02-12.054 8.894-20.538 6.652a21.09 21.09 0 0 1-1.117-.33c-.113-.035-.224-.072-.336-.1a22.36 22.36 0 0 1-.781-.274l-.353-.134c-.283-.1-.563-.225-.84-.345-.076-.033-.152-.063-.227-.098a19.53 19.53 0 0 1-1.03-.487c-.174-.087-.345-.178-.516-.268l-.298-.156a20.05 20.05 0 0 1-.653-.375l-.156-.1a25.46 25.46 0 0 1-.79-.492c-.08-.052-.158-.1-.238-.162l-.512-.345a27.46 27.46 0 0 1-1.066-.794l-.24-.192c-3.713-2.986-6.657-7.066-8.056-11.693-1.467-4.8-1.15-10.185 1.4-14.556m10.648-.38c-2.252 3.376-2.473 7.568-.9 11.296 1.648 3.957 5.025 7.062 8.966 8.533.162.062.325.117.5.173l.216.07c.232.074.463.16.702.206 10.892 2.143 13.846-5.692 14.632-6.845-2.588 3.795-6.937 4.706-12.273 3.387-.42-.105-.885-.26-1.3-.406a15.62 15.62 0 0 1-1.533-.649 15.81 15.81 0 0 1-2.688-1.671C52.167 12.8 49.2 5.762 52.316.03"
                                                        fill="#0868ac"/>
                                                    <g fill="#FFFFFF">
                                                        <path
                                                            d="M26.576 74.06l-.738 2.616.738-2.615zm3.796 5.678l-.813-.005.813.005zm-.2 3.906l-4.872.018 4.872-.018zm1.02-3.9l-.814-.005.814.005zm-.582 3.568l.85-3.237-.85 3.237zm17.93-14.907l-1.58 7.433 1.58-7.433zm-4.065 0l-1.2 5.553 1.2-5.553z"/>
                                                        <path
                                                            d="M48.26 68.07h-3.38c-.188 0-.374.15-.414.334l-2.4 11.107c-.04.183-.226.333-.413.333H39.26c-2.368 0-2.094-1.637-1.6-3.88l.015-.068.287-1.53.124-.63 1.092-5.332c.038-.184-.085-.335-.273-.335h-3.47a.44.44 0 0 0-.412.334l-1.563 7.414c-.86 3.924-.632 7.666 4.04 7.783l.135.003h7.332c.188 0 .373-.15.413-.334l3.162-14.866c.04-.184-.083-.334-.27-.334zm13.487 11.813c.188 0 .3.15.273.334l-.328 1.605m-.328 1.606l.328-1.606-.328 1.606zm-.412.338l-6.23.03 6.23-.03z"/>
                                                        <path
                                                            d="M52.704 77.817c-.003-.176.197-.478.385-.478l-.422-.007c-.2 1.914.037.485.037.485zm2.326 5.978h-.065.065zm6.717-3.912c.188 0 .3.15.273.334l-.382 1.866M56.63 83.8h-.014.014zm-.83-.006h-.048.048zm-.253.001h-.08.08zm-.247 0h-.07.07zm.462-.001h-.205.205z"/>
                                                        <path
                                                            d="M56.617 83.8l-.816.003.816-.003zm4.337-.025l-4.325.026 4.325-.026zm.4-.347l.275-1.344-.275 1.345zm-5.896.367H55.3h.178zm-.495 0h-.24.24zm.257 0h-.2.2zM5.76 77.857l.525-2.328-.6 2.66-.07.334.146-.668zm6.286-9.825H8.333a.45.45 0 0 0-.417.333l-.704 3.1a.26.26 0 0 0 .266.333h3.742c.188 0 .374-.15.414-.333l.68-3.107c.04-.183-.08-.333-.27-.333zm-.808 5.168l-1.1 5.038 1.1-5.038zM.452 89.895l3.062.024c-.904 0-2.397-.017-3.063-.025z"/>
                                                        <path
                                                            d="M6.8 73.2l-.526 2.328L6.8 73.2zm4.17-.333H7.227a.45.45 0 0 0-.417.333l-1.05 4.656-.146.668-1 4.753a7.16 7.16 0 0 1-.18.657s-.7 2.08-1.874 2.057l-1.165-.022a.45.45 0 0 0-.42.326L.2 89.558a.26.26 0 0 0 .261.336l3.063.025c2.936 0 4.483-1.627 5.476-6.307l2.25-10.4c.04-.183-.082-.333-.27-.333zm53.162 10.738c-.188 0-.3-.15-.27-.334l2.815-13.186m1.367 13.185l1.14-5.628-1.14 5.628z"/>
                                                        <path
                                                            d="M63.903 83.438c-.023-.092-.01-.317.03-.5l1.336-6.26-1.408 6.593c-.04.184.082.334.27.334h.342c-.188 0-.548-.075-.57-.167zm3.92.092c-.102.04-.34.075-.528.075h.342a.44.44 0 0 0 .41-.335l.068-.334c-.037.184-.2.553-.3.594zm.79-3.074l.503-2.484-.503 2.484zm11.108-9.488l.155.64c.043.183-.076.332-.263.333"/>
                                                        <path
                                                            d="M68.112 82.936l.5-2.48-.5 2.48zM79.568 70.3l.153.656-.153-.656zm-10.452 7.672l.138-.664.537-2.515-.608 2.848-.067.33zm-2.393-8.104l-.117.55-1.336 6.26 1.408-6.593.045-.216z"/>
                                                        <path
                                                            d="M79.877 71.608l-.155-.64-.23-1c-.304-1.18-1.196-1.863-3.134-1.863l-8.92-.006a.44.44 0 0 0-.412.334l-.138.653-.2.987-2.744 12.853c-.04.184-.053.4-.03.5s.383.167.57.167h2.82c.188 0 .425-.034.528-.075s.254-.4.3-.594l1.07-5.294 1.145-5.364c.04-.183.225-.332.412-.333l8.873-.004c.187 0 .306-.15.263-.333zM91.3 65.815l-.683.003h-2.84a.73.73 0 0 0-.534.282l-6.28 9.2c-.106.155-.227.132-.27-.05l-.462-2.027a.45.45 0 0 0-.417-.333h-4.037c-.188 0-.3.147-.248.328l1.8 6.338c.052.18.055.477.01.66l-.8 3.067a.25.25 0 0 0 .257.331h4c.188 0 .38-.15.426-.33l.8-3.067a2.04 2.04 0 0 1 .29-.604L92.518 66.08c.113-.15.052-.272-.136-.27l-1.07.007zm-32.076 7.937c-.024.2-.212.35-.4.35h-5.12c-.177 0-.267-.12-.24-.27l.004-.027.023-.087c.5-1.3 1.485-2.153 3.356-2.153 2.107 0 2.518 1.03 2.375 2.187zm-1.502-5.908c-6.57 0-8.127 3.988-9 8.013-.874 4.103-.798 7.94 6 7.94H55.8l.83-.003 4.326-.026a.44.44 0 0 0 .407-.335l.657-3.212c.038-.184-.085-.334-.273-.334h-6.112c-2.43 0-3.153-.646-2.887-2.545h9.77c.16-.003.305-.1.362-.252.01-.027.02-.056.024-.085 1.45-5.47 1.034-9.157-5.18-9.157zM26.668 73.73l-.092.327c0 .001-.738 2.616-.738 2.616l-.738 2.614a.48.48 0 0 1-.434.328H20.76c-2.962 0-3.683-2.317-2.962-5.734.72-3.495 2.135-5.668 5.05-5.888 3.984-.3 4.78 2.502 3.82 5.736zm2.678 5.685s1.84-4.47 2.26-7.053c.57-3.457-1.16-8.47-7.845-8.47-6.647 0-9.533 4.786-10.634 10-1.1 5.24.342 9.836 6.95 9.8l10.086-.037a.47.47 0 0 0 .427-.332l.85-3.238a.25.25 0 0 0-.255-.332l-1.627-.01c-.16-.001-.25-.104-.232-.24.004-.025.01-.05.02-.076z"/>
                                                        <path
                                                            d="M62.25 76.424c0 .124-.1.224-.224.224s-.224-.1-.224-.224.1-.224.224-.224.224.1.224.224z"/>
                                                    </g>
                                                </g>
                                            </svg>
                                        </div>
                                    </div>
                                </div>

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
                    </div>

                    <div data-aos="flip-right">
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

                                <br>

                                <div
                                    class="md:w-1/3 p-6 md:ml-2 bg-white dark:bg-gray-700/50 dark:bg-gradient-to-bl from-gray-700/50 via-transparent dark:ring-1 dark:ring-inset dark:ring-white/5 rounded-lg shadow-2xl shadow-gray-500/20 dark:shadow-none flex motion-safe:hover:scale-[1.01] transition-all duration-250">
                                    <div class="overflow-x-clip">
                                        <h2 class="text-2xl font-semibold text-gray-900 dark:text-white">Featured
                                            technologies used</h2>

                                        <div class="flex">
                                            <svg
                                                viewBox="0 0 62 65"
                                                fill="none"
                                                xmlns="http://www.w3.org/2000/svg"
                                                class="h-16 mt-4 w-auto"
                                            >
                                                <path
                                                    d="M61.8548 14.6253C61.8778 14.7102 61.8895 14.7978 61.8897 14.8858V28.5615C61.8898 28.737 61.8434 28.9095 61.7554 29.0614C61.6675 29.2132 61.5409 29.3392 61.3887 29.4265L49.9104 36.0351V49.1337C49.9104 49.4902 49.7209 49.8192 49.4118 49.9987L25.4519 63.7916C25.3971 63.8227 25.3372 63.8427 25.2774 63.8639C25.255 63.8714 25.2338 63.8851 25.2101 63.8913C25.0426 63.9354 24.8666 63.9354 24.6991 63.8913C24.6716 63.8838 24.6467 63.8689 24.6205 63.8589C24.5657 63.8389 24.5084 63.8215 24.456 63.7916L0.501061 49.9987C0.348882 49.9113 0.222437 49.7853 0.134469 49.6334C0.0465019 49.4816 0.000120578 49.3092 0 49.1337L0 8.10652C0 8.01678 0.0124642 7.92953 0.0348998 7.84477C0.0423783 7.8161 0.0598282 7.78993 0.0697995 7.76126C0.0884958 7.70891 0.105946 7.65531 0.133367 7.6067C0.152063 7.5743 0.179485 7.54812 0.20192 7.51821C0.230588 7.47832 0.256763 7.43719 0.290416 7.40229C0.319084 7.37362 0.356476 7.35243 0.388883 7.32751C0.425029 7.29759 0.457436 7.26518 0.498568 7.2415L12.4779 0.345059C12.6296 0.257786 12.8015 0.211853 12.9765 0.211853C13.1515 0.211853 13.3234 0.257786 13.475 0.345059L25.4531 7.2415H25.4556C25.4955 7.26643 25.5292 7.29759 25.5653 7.32626C25.5977 7.35119 25.6339 7.37362 25.6625 7.40104C25.6974 7.43719 25.7224 7.47832 25.7523 7.51821C25.7735 7.54812 25.8021 7.5743 25.8196 7.6067C25.8483 7.65656 25.8645 7.70891 25.8844 7.76126C25.8944 7.78993 25.9118 7.8161 25.9193 7.84602C25.9423 7.93096 25.954 8.01853 25.9542 8.10652V33.7317L35.9355 27.9844V14.8846C35.9355 14.7973 35.948 14.7088 35.9704 14.6253C35.9792 14.5954 35.9954 14.5692 36.0053 14.5405C36.0253 14.4882 36.0427 14.4346 36.0702 14.386C36.0888 14.3536 36.1163 14.3274 36.1375 14.2975C36.1674 14.2576 36.1923 14.2165 36.2272 14.1816C36.2559 14.1529 36.292 14.1317 36.3244 14.1068C36.3618 14.0769 36.3942 14.0445 36.4341 14.0208L48.4147 7.12434C48.5663 7.03694 48.7383 6.99094 48.9133 6.99094C49.0883 6.99094 49.2602 7.03694 49.4118 7.12434L61.3899 14.0208C61.4323 14.0457 61.4647 14.0769 61.5021 14.1055C61.5333 14.1305 61.5694 14.1529 61.5981 14.1803C61.633 14.2165 61.6579 14.2576 61.6878 14.2975C61.7103 14.3274 61.7377 14.3536 61.7551 14.386C61.7838 14.4346 61.8 14.4882 61.8199 14.5405C61.8312 14.5692 61.8474 14.5954 61.8548 14.6253ZM59.893 27.9844V16.6121L55.7013 19.0252L49.9104 22.3593V33.7317L59.8942 27.9844H59.893ZM47.9149 48.5566V37.1768L42.2187 40.4299L25.953 49.7133V61.2003L47.9149 48.5566ZM1.99677 9.83281V48.5566L23.9562 61.199V49.7145L12.4841 43.2219L12.4804 43.2194L12.4754 43.2169C12.4368 43.1945 12.4044 43.1621 12.3682 43.1347C12.3371 43.1097 12.3009 43.0898 12.2735 43.0624L12.271 43.0586C12.2386 43.0275 12.2162 42.9888 12.1887 42.9539C12.1638 42.9203 12.1339 42.8916 12.114 42.8567L12.1127 42.853C12.0903 42.8156 12.0766 42.7707 12.0604 42.7283C12.0442 42.6909 12.023 42.656 12.013 42.6161C12.0005 42.5688 11.998 42.5177 11.9931 42.4691C11.9881 42.4317 11.9781 42.3943 11.9781 42.3569V15.5801L6.18848 12.2446L1.99677 9.83281ZM12.9777 2.36177L2.99764 8.10652L12.9752 13.8513L22.9541 8.10527L12.9752 2.36177H12.9777ZM18.1678 38.2138L23.9574 34.8809V9.83281L19.7657 12.2459L13.9749 15.5801V40.6281L18.1678 38.2138ZM48.9133 9.14105L38.9344 14.8858L48.9133 20.6305L58.8909 14.8846L48.9133 9.14105ZM47.9149 22.3593L42.124 19.0252L37.9323 16.6121V27.9844L43.7219 31.3174L47.9149 33.7317V22.3593ZM24.9533 47.987L39.59 39.631L46.9065 35.4555L36.9352 29.7145L25.4544 36.3242L14.9907 42.3482L24.9533 47.987Z"
                                                    fill="#FF2D20"
                                                />
                                            </svg>

                                            <svg xmlns="http://www.w3.org/2000/svg" width="75" height="75" class="mt-3"
                                                 viewBox="0 0 48 48">
                                                <polygon fill="#40c4ff" points="26,4 6,24 12,30 38,4"></polygon>
                                                <polygon fill="#40c4ff" points="38,22 27,33 21,27 26,22"></polygon>
                                                <rect width="8.485" height="8.485" x="16.757" y="28.757" fill="#03a9f4"
                                                      transform="rotate(-45.001 21 33)"></rect>
                                                <polygon fill="#01579b" points="38,44 26,44 21,39 27,33"></polygon>
                                                <polygon fill="#084994" points="21,39 30,36 27,33"></polygon>
                                            </svg>
                                        </div>
                                    </div>
                                </div>

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
        </div>
    </section>

    <div class="bg-gradient-to-l from-blue-400 to-teal-400">
        <br>
    </div>

    <section id="experience"
             class="relative sm:flex sm:justify-center sm:items-center min-h-screen bg-dots-darker bg-center bg-gray-100 dark:bg-dots-lighter dark:bg-gray-900 selection:bg-red-500 selection:text-white">
        <div class="max-w-7xl mx-auto p-6 lg:p-8">
            <div class="flex justify-center text-justify md:text-center">
                <div data-aos="fade-left"
                     data-aos-offset="300"
                     data-aos-easing="ease-in-sine">
                    <p class="mt-6 md:mt-16 text-4xl md:text-5xl font-semibold text-gray-900 dark:text-white">💼 Work Experience</p>
                    <p class="mt-6 text-xl w-full md:px-60 font-semibold text-gray-900 dark:text-gray-300">
                        I have previously worked on freelance web and mobile application development projects as a
                        full-stack developer, and held
                        a full-time job as a full-stack developer.
                    </p>
                </div>
            </div>

            <div class="mt-16 mb-10" data-aos="flip-left">
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
             class="relative sm:flex sm:justify-center sm:items-center min-h-screen bg-at-sign bg-center bg-gray-100 dark:bg-at-sign dark:bg-gray-900 selection:bg-red-500 selection:text-white">
        <div class="max-w-7xl mx-auto p-6 lg:p-8">
            <div class="mt-16 md:mt-4">
                <p class="mt-8 text-5xl md:text-6xl font-semibold text-gray-900 dark:text-white">Let's get in touch</p>
                <p class="mt-8 text-6xl md:text-8xl font-semibold text-gray-900 dark:text-gray-400">Have any project ideas?</p>
                <p class="mt-8 text-6xl md:text-8xl font-semibold text-gray-900 dark:text-gray-400">Have any question?</p>

                <div class="md:w-1/2 flex items-center mt-24">
                    <div
                        class="h-24 md:h-32 w-24 md:w-32 bg-white-50 dark:bg-white flex items-center justify-center rounded-full overflow-hidden">
                        <img width="250"
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
    .dark\:bg-at-sign {
        background-image: url("data:image/svg+xml,%3Csvg width='100' height='50' viewBox='0 0 30 30' fill='none' xmlns='http://www.w3.org/2000/svg'%3E%3Ctext x='0' y='20' font-family='Arial' font-size='12' fill='rgba(255,255,255,0.07)'%3E@ @ @ @%3C/text%3E%3C/svg%3E");
    }
}
</style>
