<template>
    <div class="task-input w-[60%] flex justify-center items-center flex-col gap-y-6 max-md:w-[100%] max-lg:w-[90%]">
        <div class="flex flex-col w-[50%] gap-y-1 max-md:w-[90%] max-lg:w-[80%]">
            <label for="task">Task Name</label>
            <input type="text" id="task"
                class="p-3 border-2 border-gray-400-200 top-7 rounded-lg shadow-[0_8px_14px_1px_rgba(96,165,250,0.1)] outline-none"
                placeholder="Enter Task...">
        </div>
        <div class="flex justify-between w-[50%] gap-y-1 max-md:w-[90%] max-lg:w-[80%]">
            <div class="flex flex-col w-[45%] max-lg:w-[48%]">
                <label for="from-time">From</label>
                <input type="time" id="from-time"
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
            <input type="text" id="assigned"
                class="p-3 border-2 border-gray-400-200 top-7 rounded-lg shadow-[0_8px_14px_1px_rgba(96,165,250,0.1)] outline-none"
                placeholder="Name">
        </div>
    </div>
</template>
<script>
export default {

}
</script>
<style scoped>
.form {
    border: 1px solid red;
    width: 50%;
    text-align: center;
}
</style>