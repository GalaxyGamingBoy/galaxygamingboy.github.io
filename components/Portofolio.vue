<script setup>
import l from "~/assets/layout.json"
</script>

<template>
    <ProjectShowcase :data="l.working_on">What I have been working on</ProjectShowcase>
    <ProjectShowcase :data="l.portofolio">My Portofolio</ProjectShowcase>
</template>