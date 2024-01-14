<template>
    <div v-if="toggleImg == true"
        class="z-10 absolute w-full h-full border bg-gray-800/[.3] flex justify-center items-center flex-col gap-4">
        <span class="material-symbols-outlined self-end mr-4 text-red-500 cursor-pointer text-4xl max-md:text-3xl"
            @click="closeImg">
            cancel
        </span>
        <img src="/imgs/matrix.png" alt="Image" class="w-[40%] max-md:w-[90%]">
        <p class="text-white text-center mx-4 italic">
            "The image above presents a framework to guide you in creating a productive to-do list for the day!"
        </p>
    </div>
    <div v-else class="absolute top-20 w-full h-12 flex justify-end items-center pr-20 max-md:pr-8">
        <div class="flex gap-1 invisible hover:visible transition-all" @click="showImg">
            <div class="text border border-blue-400 px-3 rounded-full shadow-[0_2px_14px_1px_rgba(0,0,0,0.05)]">
                <p class="text-sm font-light">Info</p>
            </div>
            <span
                class="material-symbols-outlined cursor-pointer hover:text-yellow-400 hover:scale-110 transition-transform visible">
                lightbulb
            </span>
        </div>
    </div>
</template>
<script setup>
import { ref } from 'vue';

let toggleImg = ref(false);

// Function to display image on click event
const showImg = () => {
    toggleImg.value = !toggleImg.value;
}

// Function to hide image on click event
const closeImg = () => {
    toggleImg.value = false;
}
</script>
<style></style>