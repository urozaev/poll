<script setup lang="ts">
import type { NuxtError } from '#app';

const { error } = defineProps<{error: NuxtError}>();

const goHome = () => {
    navigateTo('/');
}
</script>
<template>
    <div>
        <h1>{{ error.statusCode }}</h1>
        <div style="color: red">{{ error.statusMessage }}</div>
        <ActionButton color="gray" @click="goHome">На Главную</ActionButton>
    </div>
</template>