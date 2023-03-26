<script setup lang="ts">
defineProps(['link', 'linkClass'])
</script>

<template>
    <li class="nav-item">
        <NuxtLink class="nav-link" :class="linkClass" :to="link">
            <slot></slot>
        </NuxtLink>
    </li>
</template>