<template>
    <button v-if="toggleForm == false"
        class="block bg-blue-400 rounded-3xl px-4 py-2 w-[20%] max-lg:w-[50%] text-white text-lg hover:scale-95 transition-transform"
        @click="displayForm">
        Add Task
    </button>
    <div v-if="toggleForm == true" class="w-full mx-auto flex justify-center items-center">
        <form class="w-[60%] flex justify-center items-center flex-col gap-y-6 max-md:w-[100%] max-lg:w-[90%] lg:w-[90%]">
            <div class="flex flex-col w-[50%] gap-y-1 max-md:w-[90%] max-lg:w-[80%]">
                <label for="task">Task Name</label>
                <input type="text" id="task" v-model="taskName" required
                    class="p-3 border-2 border-gray-400-200 top-7 rounded-lg shadow-[0_8px_14px_1px_rgba(96,165,250,0.1)] outline-none"
                    placeholder="Enter Task...">
            </div>
            <div class="flex justify-between w-[50%] gap-y-1 max-md:w-[90%] max-lg:w-[80%]">
                <div class="flex flex-col w-[45%] max-lg:w-[48%]">
                    <label for="from-time">From</label>
                    <input type="time" id="from-time" required
                        class="p-3 border-2 border-gray-400-200 top-7 rounded-lg shadow-[0_8px_14px_1px_rgba(96,165,250,0.1)] outline-none"
                        placeholder="Enter Task...">
                </div>
                <div class="flex flex-col w-[45%] max-lg:w-[48%]">
                    <label for="to-time">To</label>
                    <input type="time" id="to-time"
                        class="p-3 border-2 border-gray-400-200 top-7 rounded-lg shadow-[0_8px_14px_1px_rgba(96,165,250,0.1)] outline-none"
                        placeholder="Enter Task...">
                </div>
            </div>
            <div class="flex flex-col w-[50%] gap-y-1 max-md:w-[90%] max-lg:w-[80%]">
                <label for="assigned">Assigned To <span class="font-light text-gray-400">(optional)</span></label>
                <input type="text" id="assigned" v-model="assignedTo"
                    class="p-3 border-2 border-gray-400-200 top-7 rounded-lg shadow-[0_8px_14px_1px_rgba(96,165,250,0.1)] outline-none"
                    placeholder="Name">
            </div>
            <div class="flex justify-end items-center mt-4 w-[50%] max-md:w-[90%] max-lg:w-[80%] gap-4">
                <button type="submit"
                    class="bg-green-400 rounded-3xl px-4 py-2 self-end w-[20%] max-lg:w-[30%] text-white text-lg hover:scale-95 transition-transform"
                    @click="saveData">
                    Save
                </button>
                <button
                    class="bg-red-400 rounded-3xl px-4 py-2 self-end w-[20%] max-lg:w-[30%] text-white text-lg hover:scale-95 transition-transform"
                    @click="hideForm">
                    Cancel
                </button>
            </div>
        </form>
    </div>
</template>
<script setup>
import { ref } from 'vue';
let taskName, assignedTo;
let toggleForm = ref(false);

const displayForm = () => {
    toggleForm.value = !toggleForm.value;
}

const hideForm = () => {
    toggleForm.value = false;
}

const saveData = () => {
    console.log(taskName);
}

</script>
<style></style>