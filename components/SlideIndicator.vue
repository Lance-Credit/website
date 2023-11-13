<template>
    <div class="indicator h-2 rounded-md cursor-pointer" :class="active ? 'w-8 bg-['+activeColor+']' : 'w-2 bg-['+defaultColor+']'"></div>
</template>

<script setup lang="ts">
    defineProps<{
        active: boolean,
        defaultColor: string,
        activeColor: string
    }>()
</script>