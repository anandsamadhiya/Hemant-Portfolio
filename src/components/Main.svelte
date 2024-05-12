<script>
    let benefits = [
        {
            metric: "10x",
            name: "a self taught developer",
            description:
                "I taught myself to code using free online resources and absolutely fell in love with the creativity and problem solving that is involved in developing and engineering innovative new online experiences. Starting of with JavaScript, HTML & CSS and evolving my knowledge base to include JavaScript frameworks, backend programming, design, cloud services and much much more.",
        },
        {
            name: "a product design & UX fanatic",
            description:
                "Carefully crafting and designing amazing user experiences allows me to express and experiment with every morsel of creativity I have. I love the challenge of learning new design concepts and enabling users with amazing online experiences.",
        },
        {
            name: "an excellent communicator",
            description:
                "Communication is key and it's a paramount value of mine. I believe in transparency and constructive communication above all else. This helps me develop deep relationships and ensures my effectiveness and productivity in any work space with any team.",
        },
    ];
    const skills = [
        { name: "HTML", image: "images/html.png" },
        { name: "CSS", image: "images/css.png" },
        {
            name: "JavaScript",
            image: "https://upload.wikimedia.org/wikipedia/commons/6/6a/JavaScript-logo.png",
        },
        { name: "Svelte", image: "images/svelte.png" },
        { name: "Tailwind CSS", image: "images/tailwindcss.png" },
    ];

    //Loading page script..
    import { onMount } from "svelte";
    import { fly } from "svelte/transition";

    let counter = 0;
    let loaderVisible = true;
    let contentVisible = false;

    onMount(() => {
        const loaderTimer = setInterval(() => {
            counter++;
            if (counter === 100) {
                clearInterval(loaderTimer);
                setTimeout(() => {
                    loaderVisible = false;
                    contentVisible = true;
                }, 500);
            }
        }, 35);
    });
</script>

<!-- Loading Page -->
<div class="font-montserrat overflow-hidden">
    {#if loaderVisible}
        <div
            class="loader bg-blue-900 flex items-center justify-center fixed top-0 left-0 w-full h-full z-50 transition-opacity duration-500 ease-in-out opacity-100"
        >
            <div
                class="loader__container flex flex-col items-center text-white z-50"
            >
                <h1 class="loader__container__counter text-9xl font-bold m-0">
                    {counter}%
                </h1>
                <h2
                    class="loader__container__loading text-3xl font-semibold uppercase mt-5"
                >
                    loading...
                </h2>
                <h3
                    class=" bg-slate-900 px-2 py-1 loader__container__loading text-2xl font-semibold uppercase mt-5 rounded-lg"
                >
                    My Portfolio
                </h3>
            </div>
            <div
                class="loader__layer bg-slate-900 fixed top-0 left-0 h-full z-40"
                style="width: {counter}%"
            ></div>
        </div>
    {/if}

    {#if contentVisible}
        <div
            class="transform transition-opacity duration-500 ease-in-out"
            style="display: block;"
            transition:fly={{ x: "-100%", duration: 500 }}
        >
            <main class="flex flex-col flex-1 p-4">
                <section
                    id="introPage"
                    class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14"
                >
                    <div
                        class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10"
                    >
                        <h2
                            class="font-semibold text-4xl sm:text-5xl md:text-6xl"
                        >
                            Hi! I'm <span class="poppins text-violet-400"
                                >Hemant</span
                            >

                            <br />Full Stack
                            <span class="poppins text-violet-400"
                                >Developer</span
                            >
                        </h2>
                        <p class="text-base sm:text-lg md:text-xl">
                            My <span class="text-violet-400">favorite tech</span
                            > includes JavaScript TailwindCSS, SvelteKit, and Firebase/Firestore!
                        </p>
                    </div>
                    <div class="relative shadow-2xl grid place-items-center">
                        <img
                            src="https://t3.ftcdn.net/jpg/03/86/83/28/360_F_386832865_KzXYSvOLzUhztbeVD5d6pi2MBMqwBGAL.jpg"
                            class="object-cover z-[2] w-full max-h-[70vh] bg-center rounded-xl"
                        />
                    </div>
                </section>
                <div
                    class="text-lg sm:text-xl md:text-6xl text-center flex justify-center font-bold"
                >
                    <span class="border-b-2"> A few of my creative work's</span>
                </div>
                <!-- Project Section -->
                <section
                    class="py-20 lg:py-32 flex flex-col gap-24"
                    id="projects"
                >
                    <div
                        class="flex flex-col sm:flex-row gap-4 text-center w-full"
                    >
                        <a href="Plus" class="shadow-2xl relative flex-1">
                            <div
                                class="h-64 relative shadow-2xl shadow-slate-900 overflow-hidden group"
                            >
                                <div
                                    class="absolute -bottom-10 group-hover:top-0 left-0 w-full h-full group-hover:bg-red-900 transition-all ease-in-out duration-500"
                                >
                                    <div class="w-full h-full p-5 relative">
                                        <div
                                            class="absolute bottom-0 group-hover:bottom-24 text-white text-left transition-all ease-in-out duration-500"
                                        >
                                            <h2
                                                class="text-2xl font-bold text-slate-900 mb-0 pb-1"
                                            >
                                                ExamPlus
                                            </h2>
                                            <p
                                                class="text-lg font-light text-white"
                                            >
                                                In this project used Java and
                                                Android Studio and <br
                                                />javascript.
                                            </p>
                                        </div>
                                    </div>
                                </div>
                                <img
                                    src="images/ExamPlus.jpeg"
                                    class="w-full h-full object-cover border border-gray-600"
                                />
                            </div>
                        </a>

                        <a href="chatui" class="shadow-2xl relative flex-1">
                            <div
                                class="h-64 relative shadow-2xl shadow-slate-900 overflow-hidden group"
                            >
                                <div
                                    class="absolute -bottom-10 group-hover:top-0 left-0 w-full h-full group-hover:bg-pink-900 transition-all ease-in-out duration-500"
                                >
                                    <div class="w-full h-full p-5 relative">
                                        <div
                                            class="absolute bottom-0 group-hover:bottom-24 text-white text-left transition-all ease-in-out duration-500"
                                        >
                                            <h2
                                                class="text-2xl font-bold text-slate-900 mb-0 pb-1"
                                            >
                                                ChatUi
                                            </h2>
                                            <p
                                                class="text-lg font-light text-white"
                                            >
                                                In this project used svelte and
                                                Tailwind and <br />javascript.
                                            </p>
                                        </div>
                                    </div>
                                </div>
                                <img
                                    src="images/Chat.png"
                                    class="w-full h-full object-cover border border-gray-600"
                                />
                            </div>
                        </a>

                        <a href="Clon" class="shadow-2xl relative flex-1">
                            <div
                                class="h-64 relative shadow-2xl shadow-slate-900 overflow-hidden group"
                            >
                                <div
                                    class="absolute -bottom-10 group-hover:top-0 left-0 w-full h-full group-hover:bg-blue-900 transition-all ease-in-out duration-500"
                                >
                                    <div class="w-full h-full p-5 relative">
                                        <div
                                            class="absolute bottom-0 group-hover:bottom-24 text-white text-left transition-all ease-in-out duration-500"
                                        >
                                            <h2
                                                class="text-2xl font-bold text-slate-900 mb-0 pb-1"
                                            >
                                                Teniflex
                                            </h2>
                                            <p
                                                class="text-lg font-light text-white"
                                            >
                                                In this project used svelte and
                                                Tailwind and <br />javascript.
                                            </p>
                                        </div>
                                    </div>
                                </div>
                                <img
                                    src="images/Screen.png"
                                    class="w-full h-full object-cover border border-gray-600"
                                />
                            </div>
                        </a>
                    </div>
                </section>

                <section
                    id="about"
                    class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative"
                >
                    <div
                        class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4"
                    >
                        <h6 class="text-large sm:text-xl md:text-2xl">
                            Want to know more?
                        </h6>
                        <h3
                            class="font-semibold text-3xl sm:text-4xl md:text-5xl"
                        >
                            A bit <span class="poppins text-violet-400"
                                >about</span
                            >
                            me.
                        </h3>
                    </div>
                    <p
                        class="mx-auto poppins font-semibold text-lg sm:text-xl md:text-2xl"
                    >
                        I am . . .
                    </p>
                    <div
                        class="flex flex-col gap-20 w-full mx-auto max-w-[800px]"
                    >
                        {#each benefits as benefit, index}
                            <div class="flex flex-col gap-6 sm:gap-8">
                                <p
                                    class="poppins text-4xl sm:text-5xl md:text-6xl text-slate-500 font-semibold"
                                >
                                    0{index + 1}
                                </p>
                                <div class="flex flex-col gap-6 sm:gap-8">
                                    <h3
                                        class="text-2xl sm:text-3xl md:text-5xl"
                                    >
                                        {benefit.name}
                                    </h3>
                                    <p>{benefit.description}</p>
                                </div>
                            </div>
                        {/each}
                    </div>
                </section>
                <section class="py-4 sm:pl-80" id="skills">
                    <div class="max-w-4xl mx-auto">
                        <h2
                            class="text-3xl font-bold text-center mb-6 text-white sm:pr-80"
                        >
                            Skills
                        </h2>

                        <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
                            <div
                                class="bg-white bg-opacity-25 shadow rounded-lg overflow-hidden hover:shadow-xl transition duration-300 relative backdrop-filter backdrop-blur-lg"
                            >
                                <div class="p-6">
                                    <h3
                                        class="text-xl font-semibold mb-2 text-white"
                                    >
                                        Development
                                    </h3>
                                    <ul
                                        class="list-disc list-inside text-white"
                                    >
                                        <li>Tailwind</li>
                                        <li>CSS</li>
                                        <li>JavaScript</li>
                                        <li>Android Studio</li>
                                        <li>Firebase</li>
                                    </ul>
                                </div>
                            </div>

                            <div
                                class="bg-white bg-opacity-25 shadow rounded-lg overflow-hidden hover:shadow-xl transition duration-300 relative backdrop-filter backdrop-blur-lg"
                            >
                                <div class="p-6">
                                    <h3
                                        class="text-xl font-semibold mb-2 text-white"
                                    >
                                        Design
                                    </h3>
                                    <ul
                                        class="list-disc list-inside text-white"
                                    >
                                        <li>UI/UX Design</li>
                                        <li>Figma</li>
                                    </ul>
                                </div>
                            </div>
                        </div>
                    </div>
                </section>
            </main>
        </div>
    {/if}
</div>
