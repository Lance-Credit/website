<template>
    <div class="indicator h-2 rounded-md cursor-pointer" :class="active ? 'w-8' : 'w-2'" :style="active ? `background: ${activeColor}` : `background: ${defaultColor}`"></div>
</template>

<script setup lang="ts">
    defineProps<{
        active: boolean,
        defaultColor: string,
        activeColor: string
    }>()
</script>