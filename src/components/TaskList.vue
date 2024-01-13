<template>
    <li class="border-b-2 w-full py-2 pl-2 font-mono" :class="borderColor" @click="updateStatus">
        {{ tasks.id }}. {{ tasks.name }}
    </li>
</template>
<script setup>
import { ref } from 'vue';

defineProps(['tasks']);

let borderColor = ref("border-red-400");

const updateStatus = () => {
    if (borderColor.value == "border-red-400") {
        borderColor.value = "border-green-400";
    } else {
        borderColor.value = "border-red-400";
    }
}

</script>
<style></style>