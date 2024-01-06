<template>
    <div class="task-input w-[60%] flex justify-center items-center flex-col gap-y-6">
        <div class="flex flex-col w-[50%] gap-y-1">
            <label for="task">Task Name</label>
            <input type="text" name="task"
                class="p-3 border-2 border-gray-400-200 top-7 rounded-lg shadow-[0_8px_14px_1px_rgba(96,165,250,0.1)] outline-none"
                placeholder="Enter Task...">
        </div>
        <div class="flex justify-between w-[50%] gap-y-1">
            <div class="flex flex-col w-[45%]">
                <label for="from-time">From</label>
                <input type="time" name="from-time"
                    class="p-3 border-2 border-gray-400-200 top-7 rounded-lg shadow-[0_8px_14px_1px_rgba(96,165,250,0.1)] outline-none"
                    placeholder="Enter Task...">
            </div>
            <div class="flex flex-col w-[45%]">
                <label for="to-time">To</label>
                <input type="time" name="to-time"
                    class="p-3 border-2 border-gray-400-200 top-7 rounded-lg shadow-[0_8px_14px_1px_rgba(96,165,250,0.1)] outline-none"
                    placeholder="Enter Task...">
            </div>
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
<!-- 96 165 250 / 0.3 -->