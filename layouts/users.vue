<template>
    <header class="bg-dark p-3">
        <ul class="nav">
            <li><NuxtLink to="/" class="nav-link text-white">Главная</NuxtLink></li>
            <li><NuxtLink to="/contact" class="nav-link text-white">Контакты</NuxtLink></li>
            <li><NuxtLink to="/users/" class="nav-link text-white">Пользователи</NuxtLink></li>
        </ul>
    </header>

    <div class="container py-5">
        <slot />
    </div>

    <footer class="bg-dark p-3">
        <p class="text-white">All right reserved &copy;</p>
    </footer>
</template>

<style scoped>
    header a:not(.route-link-exact-active):hover{
        text-decoration: underline;
    }

    header a.router-link-exact-active{
        color: #ffb636!important;
        font-weight: 500;
    }
</style>