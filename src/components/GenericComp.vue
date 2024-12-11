<script setup lang="ts">
    import { ref, Ref } from 'vue'
    const { msg = 'hello'} = defineProps<{ msg?: string }>()
    const year: Ref<string | number> = ref(2020)
</script>

<template>
    <div class="box">
        <h1>TypeScript Fun</h1>
        <div>Parent Sent: {{ msg }}</div>
        {{ year }}
    </div>
</template>

<style scoped>
/* Your component styles go here */
</style>