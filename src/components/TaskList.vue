<template>
    <li class="border-b-2 w-full py-2 pl-2 font-mono">
        {{ tasks.id }}. {{ tasks.name }}
    </li>
</template>
<script setup>
defineProps(['tasks'])
</script>
<style></style>