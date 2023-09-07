<template>
    <div>
        <div>
            <slot></slot>
        </div>

        <div v-if="props?.errors?.length"></div>
    </div>
</template>

<script setup lang="ts">
    const props = defineProps<{
        errors?: any[]
    }>()
</script>
