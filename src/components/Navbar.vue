<template>
        <nav class="navbar navbar-expand-lg navbar-dark bg-success">
            <div class="container-fluid">
            <a class="navbar-brand" href="#">Vue Site</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                <li class="nav-item">
                    <RouterLink to="/" :class="['nav-link', $route.path === '/' ? 'active' : '']">Home</RouterLink>
                </li>
                <li class="nav-item">
                    <RouterLink to="/about" :class="['nav-link', $route.path === '/about' ? 'active' : '']">About</RouterLink>
                </li>
                <li class="nav-item">
                    <RouterLink to="/beatlesalbums" :class="['nav-link', $route.path === '/beatlesalbums' ? 'active' : '']">Beatles Albums</RouterLink>
                </li>
            </ul>
            </div>
        </div>
        </nav>
</template>