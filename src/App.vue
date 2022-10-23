<script setup>
import avatarUrl from "./assets/images/avatar.png";

const items = [
	{
		title: 'Headers',
		description:
			'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore.',
		icon: 'flat-color-icons:home',
	},
	{
		title: 'Footers',
		description:
			'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore.',
		icon: 'flat-color-icons:faq',
	},
	{
		title: 'Features',
		description:
			'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore.',
		icon: 'flat-color-icons:video-projector',
	},
	{
		title: 'Call-to-Action',
		description:
			'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore.',
		icon: 'flat-color-icons:video-projector',
	},
	{
		title: 'Pricing',
		description:
			'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore.',
		icon: 'flat-color-icons:calculator',
	},
	{
		title: 'Testimonial',
		description:
			'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore.',
		icon: 'flat-color-icons:voice-presentation',
	},
];
</script>

<template>
    <header
        class="sticky top-0 z-40 flex-none mx-auto w-full bg-white md:bg-white/90 dark:bg-slate-900 dark:md:bg-slate-900/90 md:backdrop-blur-sm border-b dark:border-b-0">
        <div class="py-3 px-3 mx-auto w-full md:flex md:justify-between max-w-6xl md:px-4">
            <div class="flex justify-between">
                <div class="flex items-center md:hidden">
                    <button type="button"
                        class="text-gray-500 dark:text-gray-400 hover:bg-gray-100 dark:hover:bg-gray-700 focus:outline-none focus:ring-4 focus:ring-gray-200 dark:focus:ring-gray-700 rounded-lg text-sm p-2.5 inline-flex items-center"
                        aria-label="Toggle between Dark and Light mode" data-aw-toggle-color-scheme="">
                        <svg viewBox="0 0 24 24" class="w-6 h-6" astro-icon="tabler:sun">
                            <g fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
                                stroke-width="2" class="icon-tabler">
                                <circle cx="12" cy="12" r="4"></circle>
                                <path d="M3 12h1m8-9v1m8 8h1m-9 8v1M5.6 5.6l.7.7m12.1-.7-.7.7m0 11.4.7.7m-12.1-.7-.7.7">
                                </path>
                            </g>
                        </svg>
                    </button>
                    <button type="button"
                        class="ml-1.5 text-gray-500 dark:text-gray-400 hover:bg-gray-100 dark:hover:bg-gray-800 focus:outline-none focus:ring-4 focus:ring-gray-200 dark:focus:ring-gray-700 rounded-lg text-sm p-2.5 inline-flex items-center transition"
                        aria-label="Toggle Menu" data-aw-toggle-menu="">
                        <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"
                            preserveAspectRatio="xMidYMid meet" viewBox="0 0 24 24" class="w-6 h-6"
                            astro-icon="tabler:menu">
                            <g class="icon-tabler" fill="none" stroke="currentColor" stroke-width="2"
                                stroke-linecap="round" stroke-linejoin="round">
                                <path d="M4 8h16"></path>
                                <path d="M4 16h16"></path>
                            </g>
                        </svg>
                    </button>
                </div>
            </div>
            <nav class="items-center w-full md:w-auto hidden md:flex text-gray-600 dark:text-slate-200 h-screen md:h-auto"
                aria-label="Main navigation" id="menu">
                <ul class="flex flex-col pt-8 md:pt-0 md:flex-row md:self-center w-full md:w-auto text-xl md:text-base">
                    <!-- <li>
					<a
						class="font-medium hover:text-gray-900 dark:hover:text-white px-4 py-3 flex items-center transition duration-150 ease-in-out"
						href="#">Pages</a
					>
				</li> -->
                    <!-- <li>
					<a
						class="font-medium hover:text-gray-900 dark:hover:text-white px-4 py-3 flex items-center transition duration-150 ease-in-out"
						href={getPermalink('useful-resources-to-create-websites', 'post')}
						>Resources
					</a>
				</li> -->
                    <!-- <li>
					<a
						class="font-medium hover:text-gray-900 dark:hover:text-white px-4 py-3 flex items-center transition duration-150 ease-in-out"
						href={getBlogPermalink()}>Blog</a
					>
				</li> -->
                    <li class="md:hidden">
                        <a class="font-bold hover:text-gray-900 dark:hover:text-white px-4 py-3 flex items-center transition duration-150 ease-in-out"
                            href="https://github.com/luismgsantos">Github
                        </a>
                    </li>
                </ul>
                <div class="md:self-center flex items-center mb-4 md:mb-0 ml-2">
                    <div class="hidden items-center md:flex">
                        <button type="button"
                            class="text-gray-500 dark:text-gray-400 hover:bg-gray-100 dark:hover:bg-gray-700 focus:outline-none focus:ring-4 focus:ring-gray-200 dark:focus:ring-gray-700 rounded-lg text-sm p-2.5 inline-flex items-center"
                            aria-label="Toggle between Dark and Light mode" data-aw-toggle-color-scheme="">
                            <svg viewBox="0 0 24 24" class="w-5 h-5" astro-icon="tabler:sun">
                                <g fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
                                    stroke-width="2" class="icon-tabler">
                                    <circle cx="12" cy="12" r="4"></circle>
                                    <path
                                        d="M3 12h1m8-9v1m8 8h1m-9 8v1M5.6 5.6l.7.7m12.1-.7-.7.7m0 11.4.7.7m-12.1-.7-.7.7">
                                    </path>
                                </g>
                            </svg>
                        </button>

                        <a href="https://github.com/luismgsantos"
                            class="inline-block text-gray-500 dark:text-gray-400 hover:bg-gray-100 dark:hover:bg-gray-700 focus:outline-none focus:ring-4 focus:ring-gray-200 dark:focus:ring-gray-700 rounded-lg text-sm p-2.5"
                            aria-label="luismgsantos Github">
                            <svg viewBox="0 0 24 24" class="w-5 h-5" astro-icon="tabler:brand-github">
                                <path fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
                                    stroke-width="2"
                                    d="M9 19c-4.3 1.4-4.3-2.5-6-3m12 5v-3.5c0-1 .1-1.4-.5-2 2.8-.3 5.5-1.4 5.5-6a4.6 4.6 0 0 0-1.3-3.2 4.2 4.2 0 0 0-.1-3.2s-1.1-.3-3.5 1.3a12.3 12.3 0 0 0-6.2 0C6.5 2.8 5.4 3.1 5.4 3.1a4.2 4.2 0 0 0-.1 3.2A4.6 4.6 0 0 0 4 9.5c0 4.6 2.7 5.7 5.5 6-.6.6-.6 1.2-.5 2V21">
                                </path>
                            </svg>
                        </a>
                        <a href="https://www.linkedin.com/in/luismgsantos"
                            class="inline-block text-gray-500 dark:text-gray-400 hover:bg-gray-100 dark:hover:bg-gray-700 focus:outline-none focus:ring-4 focus:ring-gray-200 dark:focus:ring-gray-700 rounded-lg text-sm p-2.5"
                            aria-label="luismgsantos linkedin">
                            <svg viewBox="0 0 24 24" class="w-5 h-5" astro-icon="tabler:brand-linkedin">
                                <g fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
                                    stroke-width="2" class="icon-tabler">
                                    <rect width="16" height="16" x="4" y="4" rx="2"></rect>
                                    <path d="M8 11v5M8 8v.01M12 16v-5M16 16v-3a2 2 0 0 0-4 0"></path>
                                </g>
                            </svg>
                        </a>
                    </div>
                </div>
            </nav>
        </div>
    </header>

    <section>
        <div class="mx-auto max-w-screen-lg px-3 py-6">
            <div class="flex flex-col items-center md:flex-row md:justify-between md:gap-x-24">
                <div>
                    <h1 class="text-3xl font-bold">
                        Hey hey, I'm
                        <span
                            class="bg-gradient-to-r from-primary-500 to-secondary-500 bg-clip-text text-transparent">Luís</span>
                        👋
                    </h1>
                    <p class="mt-6 text-xl leading-9">
                        <span class="text-primary-500 bg-clip-text text-transparent">Fullstack Developer</span>
                        using Laravel ecosystem to build software ❤️ <br />
                        Growing as a
                        <a href="https://www.digitalocean.com/community/conceptual-articles/s-o-l-i-d-the-first-five-principles-of-object-oriented-design"
                            class="hover:text-primary-600 underline underline-offseFt-4 decoration-1 decoration-dotted transition ease-in duration-200"
                            target="_blank">SOLID</a>
                        developer everyday 💻 <br />
                        Compulsive seeker of the "Aha! moment" 💡<br />
                        Always looking for new challenges 🚀
                    </p>
                </div>
                <div class="shrink-0">
                    <img :src="avatarUrl" alt="avatar picture" />
                </div>
            </div>
        </div>
    </section>

    <section class="relative">
        <div class="absolute inset-0 bg-primary-50 dark:bg-slate-800 pointer-events-none mb-32" aria-hidden="true">
        </div>
        <p></p>
        <div class="relative max-w-6xl mx-auto px-4 sm:px-6">
            <div class="py-4 pt-8 sm:py-6 lg:py-8 lg:pt-12">
                <div class="mb-8 text-center">
                    <h2 class="text-4xl md:text-5xl font-bold leading-tighter tracking-tighter mb-4 font-heading">
                        Recent Achievements
                    </h2>
                    <!-- timeline -->
                    <div class="container bg-primary-50 dark:bg-slate-800 mx-auto w-full h-full">
                        <div class="relative wrap overflow-hidden p-10 h-full">
                            <div class="border-2-2 absolute border-opacity-20 border-gray-700 h-full border"
                            style="left: 50%"></div>

                            <div v-for="(item, index) in items" :class="`mb-8 flex justify-between items-center w-full ${ index%2===0 ? 'right': 'left' }-timeline ${ index%2===0 ? 'flex-row-reverse': '' }`">
                                <div class="order-1 w-5/12"></div>
                                <div
                                    class="z-20 flex items-center order-1 bg-gray-800 dark:bg-primary-50 shadow-xl w-8 h-8 rounded-full">
                                    <h1 class="mx-auto font-semibold text-lg text-white dark:text-gray-900">
                                        {{index + 1}}
                                    </h1>
                                </div>
                                <div class="order-1 bg-gray-400 rounded-lg shadow-xl w-5/12 px-6 py-4">
                                    <h3 class="mb-3 font-bold text-gray-800 text-xl">
                                        {{item.title}}
                                    </h3>
                                    <p class="text-sm leading-snug tracking-wide text-gray-900 text-opacity-100">
                                        {{item.description}}
                                    </p>
                                </div>
                            </div>

                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>
