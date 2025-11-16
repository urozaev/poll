<template>
    <button :class="color" class="button"><slot/></button>
</template>
<script setup lang="ts">
    const { color = 'primary' } = defineProps<{
        color: 'primary' | 'gray',
    }>();
</script>
<style scoped>
.button {
   display: flex;
    box-sizing: border-box;
    align-items: center;
    justify-content: center;
    border: none;
    cursor: pointer;
    outline: none;
    -webkit-user-select: none;
    user-select: none;
    white-space: nowrap;
    max-height: 32px;
    padding: 6px 12px;
    font-size: 14px;
    font-weight: 400;
    line-height: 20px;
    border-radius: 6px;
}

.primary {
    border: 1px solid transparent;
    background-color: #06f;
    color: #fff;
}

.gray {
    border: 1px solid #D9DBDE;
    background-color: #fff;
    color: #171c22;
}
</style>
