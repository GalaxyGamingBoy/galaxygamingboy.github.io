<template>
    <nav class="navbar navbar-expand-lg bg-body-tertiary">
        <div class="container-fluid">
            <NuxtLink class="navbar-brand" to="/">Marios Mitsios</NuxtLink>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent"
                aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarSupportedContent">
                <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                    <NavbarLink link="/about" link-class="active">About Me</NavbarLink>
                    <NavbarLink link="/portofolio">My Portofolio</NavbarLink>
                </ul>
            </div>
        </div>
    </nav>
</template>