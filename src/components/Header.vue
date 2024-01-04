<template>
    <div class="header flex justify-between items-center">
        <h1 class="text-xl font-bold">To-Do</h1>
        <div class="icon">
            <a href="https://github.com/abno-24/To-Do-App" target="_blank" class="hover:fill-sky-400">
                <svg xmlns="http://www.w3.org/2000/svg" height="24" viewBox="0 -960 960 960" width="24" class="hover:scale-150 transition-transform">
                    <path
                        d="M320-240 80-480l240-240 57 57-184 184 183 183-56 56Zm320 0-57-57 184-184-183-183 56-56 240 240-240 240Z" />
                </svg>
            </a>
        </div>
    </div>
</template>
<script>
export default {

}
</script>
<style scoped>
    .header {
        position: absolute;
        top: 0;
        width: 100vw;
        height: 4rem;
        padding: 0.3rem 5rem;
        box-shadow: 0 2px 14px 1px rgba(0, 0, 0, 0.03);
    }
    /* svg:hover {
        fill: red;
    } */
</style>