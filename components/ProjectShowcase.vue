<script setup lang="ts">
defineProps(['data'])
</script>

<template>
    <div id="portofolio" class="m-5 portofolio-text">
        <h1 class="ctext">
            <slot></slot>
        </h1>
        <hr class="pshowcase-title">
        <div class="row row-cols-1 row-cols-md-2 g-4">
            <div class="col" v-for="i in data">
                <div class="card portofolio-card">
                    <img :src="i.img" class="card-img-top card-img-max-height">
                    <div class="card-body">
                        <h5 class="card-title">{{ i.name }}</h5>
                        <p class="card-text" v-html="i.desc"></p>
                        <a :href="i.repo" class="btn btn-secondary">Repository</a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>