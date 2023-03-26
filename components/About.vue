<script setup>
import l from "~/assets/layout.json"
</script>

<template>
    <div id="about" class="m-5">
        <div class="card">
            <div class="card-header">
                About Me
            </div>
            <div class="card-body">
                <div class="px-3">
                    <div class="d-flex">
                        <img src="~/public/img/me.jpg" class="rounded img-thumbnail float-md-start" style="max-width: 20%;"
                            alt="Me.png">
                        <div class="float-md-none m-3 align-self-sm-center">
                            <h5 class="card-title about-text-title">{{ l.about.about_me.title }}</h5>
                            <p class="card-text about-text" v-html="l.about.about_me.desc"></p>
                        </div>
                    </div>
                    <br>
                    <div class="float-md-none about-text">
                        <ul class="list-group">
                            <li class="list-group-item active" aria-current="true">Programming Languages that I use:
                            </li>
                            <li class="list-group-item" v-for="i in l.about.programming_languages">{{ i }}</li>
                        </ul> <br>
                        <ul class="list-group">
                            <li class="list-group-item active" aria-current="true">Code Editors that I use:</li>
                            <li class="list-group-item" v-for="i in l.about.code_editor">{{ i }}</li>

                        </ul>
                    </div>
                    <br>
                    <NuxtLink to="/portofolio" class="btn btn-secondary about-text">See my portofolio</NuxtLink>
                </div>
            </div>
        </div>
    </div>
</template>