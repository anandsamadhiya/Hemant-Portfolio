<script>
    import { fly } from "svelte/transition";

    let showText = true; // Set showText to true to make the text visible by default
</script>

<section class="relative pt-12 bg-slate-200 mb-8">
    <div class="flex flex-wrap items-center justify-center">
        <div class="w-full md:w-4/12 px-4 md:order-last relative">
            <img
                alt="..."
                class="max-w-full h-auto md:h-96 rounded-lg shadow-lg"
                src="images/Chat.png"
            />
        </div>
        <div
            class="w-full md:w-5/12 px-4 md:order-first relative md:pl-8 text-black"
            transition:fly={{ x: -100, duration: 500 }}
            style="opacity: {showText ? 1 : 0}"
        >
            <h3 class="text-3xl font-semibold">ChatUi</h3>
            <p class="mt-4 text-lg leading-relaxed text-blueGray-50">
                ChatUi is a website that can be used to chat with everyone. In
                this project used svelte and Tailwind, Firebase and <br
                />javascript. <br />This project is also used in business
                related work.
            </p>
        </div>
    </div>
</section>

<section class="relative bg-slate-200 mb-8">
    <div class="flex flex-wrap items-center justify-center">
        <div class="w-full md:w-4/12 px-4 md:order-first relative md:pr-8">
            <!-- Image on the left side -->
            <img
                alt="..."
                class="max-w-full h-auto md:h-96 rounded-lg shadow-lg"
                src="images/Demo.png"
            />
        </div>
        <div
            class="w-full md:w-5/12 px-4 md:order-last relative md:pl-8 text-black"
            transition:fly={{ x: -100, duration: 500 }}
            style="opacity: {showText ? 1 : 0}"
        >
            <h3 class="text-3xl font-semibold">Chatlist</h3>
            <p class="mt-4 text-lg leading-relaxed text-blueGray-50">
                The chat list contains all your contacts with whom you are
                talking and who are connected to you.
            </p>
        </div>
    </div>
</section>

<section class="relative bg-slate-200 mb-8">
    <div class="flex flex-wrap items-center justify-center">
        <div class="w-full md:w-4/12 px-4 md:order-last relative md:pr-8">
            <!-- Image on the left side -->
            <img
                alt="..."
                class="max-w-full h-auto md:h-96 rounded-lg shadow-lg"
                src="images/Demo1.png"
            />
        </div>
        <div
            class="w-full md:w-5/12 px-4 md:order-first relative md:pl-8 text-black"
            transition:fly={{ x: -100, duration: 500 }}
            style="opacity: {showText ? 1 : 0}"
        >
            <h3 class="text-3xl font-semibold">Sidebar</h3>
            <p class="mt-4 text-lg leading-relaxed text-blueGray-50">
                The sidebar is added inside the icon. When you click on the
                icon, the sidebar opens.
            </p>
        </div>
    </div>
</section>
