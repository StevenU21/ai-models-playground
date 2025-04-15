<script setup lang="ts">
import type { HTMLAttributes } from 'vue';

defineOptions({
    inheritAttrs: false,
});

interface Props {
    className?: HTMLAttributes['class'];
}

defineProps<Props>();
</script>   

<template>
    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" :class="className" v-bind="$attrs" fill="none">
        <rect width="24" height="24" rx="12" fill="#18181b" />
        <!-- Cabeza del bot -->
        <ellipse cx="12" cy="13" rx="6" ry="5" fill="white" />
        <!-- Ojos -->
        <circle cx="10" cy="13" r="1" fill="#18181b" />
        <circle cx="14" cy="13" r="1" fill="#18181b" />
        <!-- Boca (sonrisa) -->
        <path d="M10.5 15c.5.5 2.5.5 3 0" stroke="#18181b" stroke-width="1" stroke-linecap="round" />
        <!-- Antena -->
        <rect x="11.25" y="6" width="1.5" height="2.5" rx="0.75" fill="#fff" />
        <circle cx="12" cy="6" r="1" fill="#4f46e5" />
        <!-- Orejas -->
        <rect x="5.5" y="12" width="1" height="2" rx="0.5" fill="#fff" />
        <rect x="17.5" y="12" width="1" height="2" rx="0.5" fill="#fff" />
    </svg>
</template>
