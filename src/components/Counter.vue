<script setup lang="ts">
import { ref, computed } from 'vue';
const count = ref<number>(0);
const countMessage = computed(() => `The count is: ${count.value}`);
</script>

<template>
    <div>
        <h2>{{ countMessage }}</h2>
        <button @click="count++">Increment</button>
        <button @click="count=0">Reset</button>
    </div>
</template>


<style></style>