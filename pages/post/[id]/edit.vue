<template>
    <div>
        <h1>Editting post #{{ postNumber }}</h1>
        <div>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Repudiandae at ea dicta omnis est sit praesentium et eveniet id officia? Qui nam cumque ex repudiandae corrupti? Ipsa quibusdam ullam repudiandae?</p>
        </div>
    </div>
</template>
<script lang="ts" setup>
    const postNumber = useRoute().params.id;
</script>