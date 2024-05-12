<script>
    import { fly } from "svelte/transition";

    let showText = true; // Set showText to true to make the text visible by default
</script>

<section class="relative pt-12 bg-red-900 mb-8">
    <div class="flex flex-wrap items-center justify-center">
        <div class="w-full md:w-4/12 px-4 md:order-last relative">
            <img
                alt="..."
                class="max-w-full h-auto md:h-96 rounded-lg shadow-lg"
                src="images/Screen.png"
            />
        </div>
        <div
            class="w-full md:w-5/12 px-4 md:order-first relative md:pl-8"
            transition:fly={{ x: -100, duration: 500 }}
            style="opacity: {showText ? 1 : 0}"
        >
            <h3 class="text-3xl font-semibold">Teniflex</h3>
            <p class="mt-4 text-lg leading-relaxed text-blueGray-50">
                Teniflex is a website in which you can watch your favorite shows
                and movies. In this project used Svelte and Tailwind, Firebase
                and <br />JavaScript.
            </p>
        </div>
    </div>
</section>

<section class="relative bg-red-900 mb-8">
    <div class="flex flex-wrap items-center justify-center">
        <div class="w-full md:w-4/12 px-4 md:order-first relative md:pr-8">
            <img
                alt="..."
                class="max-w-full h-auto md:h-96 rounded-lg shadow-lg"
                src="images/Darkmode.png"
            />
        </div>
        <div
            class="w-full md:w-5/12 px-4 md:order-last relative md:pl-8"
            transition:fly={{ x: -100, duration: 500 }}
            style="opacity: {showText ? 1 : 0}"
        >
            <h3 class="text-3xl font-semibold">Darkmode</h3>
            <p class="mt-4 text-lg leading-relaxed text-blueGray-50">
                When you click on the dark mode button, the color of your screen
                changes from light mode to dark mode.
            </p>
        </div>
    </div>
</section>
