<script>
    import { fly } from "svelte/transition";

    let showText = true; // Set showText to true to make the text visible by default
</script>

<section class="relative pt-12 bg-slate-900 mb-8">
    <div class="flex flex-wrap items-center justify-center">
        <div class="w-full md:w-4/12 px-4 md:order-last relative">
            <img
                alt="..."
                class="max-w-full h-auto md:h-96 rounded-lg shadow-lg"
                src="images/ExamPlus.jpeg"
            />
        </div>
        <div
            class="w-full md:w-5/12 px-4 md:order-first relative md:pl-8"
            transition:fly={{ x: -100, duration: 500 }}
            style="opacity: {showText ? 1 : 0}"
        >
            <h3 class="text-3xl font-semibold">ExamPlus Pro</h3>
            <p class="mt-4 text-lg leading-relaxed text-blueGray-50">
                ExamPlus Pro is a software that can be used for online
                assessment. In this project used Java, Android Studio,
                Firebase/Firestore and JavaScript
            </p>
        </div>
    </div>
</section>

<section class="relative bg-slate-900 mb-8">
    <div class="flex flex-wrap items-center justify-center">
        <div class="w-full md:w-4/12 px-4 md:order-first relative md:pr-8">
            <img
                alt="..."
                class="max-w-full h-auto md:h-96 rounded-lg shadow-lg"
                src="images/ExamPlus1.jpeg"
            />
        </div>
        <div
            class="w-full md:w-5/12 px-4 md:order-last relative md:pl-8"
            transition:fly={{ x: -100, duration: 500 }}
            style="opacity: {showText ? 1 : 0}"
        >
            <h3 class="text-3xl font-semibold">ExamPlus</h3>
            <p class="mt-4 text-lg leading-relaxed text-blueGray-50">
                You can see your information here like how many questions you
                have answered correctly, your profile and your result.
            </p>
        </div>
    </div>
</section>
<section class="relative pt-12 bg-slate-900 mb-8">
    <div class="flex flex-wrap items-center justify-center">
        <div class="w-full md:w-4/12 px-4 md:order-last relative">
            <img
                alt="..."
                class="max-w-full h-auto md:h-96 rounded-lg shadow-lg"
                src="images/ExamPlus2.jpeg"
            />
        </div>
        <div
            class="w-full md:w-5/12 px-4 md:order-first relative md:pl-8"
            transition:fly={{ x: -100, duration: 500 }}
            style="opacity: {showText ? 1 : 0}"
        >
            <h3 class="text-3xl font-semibold">Question & Answer</h3>
            <p class="mt-4 text-lg leading-relaxed text-blueGray-50">
                You are asked a question, you have to select one answer from
                four answers.
            </p>
        </div>
    </div>
</section>
<section class="relative bg-slate-900 mb-8">
    <div class="flex flex-wrap items-center justify-center">
        <div class="w-full md:w-4/12 px-4 md:order-first relative md:pr-8">
            <img
                alt="..."
                class="max-w-full h-auto md:h-96 rounded-lg shadow-lg"
                src="images/ExamPlus3.jpeg"
            />
        </div>
        <div
            class="w-full md:w-5/12 px-4 md:order-last relative md:pl-8"
            transition:fly={{ x: -100, duration: 500 }}
            style="opacity: {showText ? 1 : 0}"
        >
            <h3 class="text-3xl font-semibold">Result</h3>
            <p class="mt-4 text-lg leading-relaxed text-blueGray-50">
                You get the answer to how many questions you have answered
                correctly after the time is over.
            </p>
        </div>
    </div>
</section>

<section class="relative pt-12 bg-slate-900 mb-8">
    <div class="flex flex-wrap items-center justify-center">
        <div class="w-full md:w-4/12 px-4 md:order-last relative">
            <img
                alt="..."
                class="max-w-full h-auto md:h-96 rounded-lg shadow-lg"
                src="images/ExamPlus4.jpeg"
            />
        </div>
        <div
            class="w-full md:w-5/12 px-4 md:order-first relative md:pl-8"
            transition:fly={{ x: -100, duration: 500 }}
            style="opacity: {showText ? 1 : 0}"
        >
            <h3 class="text-3xl font-semibold">Refer & Earn</h3>
            <p class="mt-4 text-lg leading-relaxed text-blueGray-50">
                When you share this software with someone, you can also win
                prizes.
            </p>
        </div>
    </div>
</section>
