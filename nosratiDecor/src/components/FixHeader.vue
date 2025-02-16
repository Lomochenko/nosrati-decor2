<script setup>
import { RouterLink } from 'vue-router';

// const navItems = [
//     {
//         title: 'خانه',
//         path: '/', text: 'صفحه اصلی'
//     },
//     {
//         title: 'محصولات',
//         path: '/products', text: 'صفحه محصولات'
//     },
// ]
</script>

<template>
    <!-- Nav Bar -->
    <div class="dsn-nav-bar">
        <div class="site-header">
            <div class="extend-container">
                <div class="inner-header">
                    <div class="main-logo">
                        <RouterLink to="/">
                            <img class="dark-logo" src="assets/img/logo-dark.png" alt="" />
                            <img class="light-logo" src="assets/img/logo.png" alt="" />
                        </RouterLink>
                    </div>
                </div>
                <nav class=" accent-menu main-navigation">
                    <ul class="extend-container">
                        <!-- home -->
                        <li class="custom-drop-down">
                            <RouterLink to="/">خانه</RouterLink>
                        </li>
                        <!-- products -->
                        <li class="custom-drop-down">
                            <RouterLink to="/products">محصولات</RouterLink>
                        </li>
                    </ul>
                </nav>
            </div>
        </div>
        <div class="header-top header-top-hamburger">
            <div class="header-container">
                <div class="logo main-logo">
                    <router-link to="/">
                        <img class="dark-logo" src="assets/img/logo-dark.png" alt="" />
                        <img class="light-logo" src="assets/img/logo.png" alt="" />
                    </router-link>
                </div>

                <div class="menu-icon" data-dsn="parallax" data-dsn-move="5">
                    <div class="icon-m">
                        <i class="menu-icon-close fas fa-times"></i>
                        <span class="menu-icon__line menu-icon__line-left"></span>
                        <span class="menu-icon__line"></span>
                        <span class="menu-icon__line menu-icon__line-right"></span>
                    </div>

                    <div class="text-menu">
                        <div class="text-button">Menu</div>
                        <div class="text-open">Open</div>
                        <div class="text-close">Close</div>
                    </div>
                </div>

                <div class="nav">
                    <div class="inner">
                        <div class="nav__content">

                        </div>
                    </div>
                </div>
                <div class="nav-content">
                    <div class="inner-content">
                        <address class="v-middle">
                            <span>Egypt</span>
                            <span>Damietta,El-Mahalla El-Kubra,</span>
                            <span>01024552406 , 01004392260</span>
                        </address>
                    </div>

                </div>
            </div>
        </div>
    </div>
    <!-- End Nav Bar -->
</template>

<style>
.dsn-nav-bar>.header-top>.header-container,
.dsn-nav-bar .site-header {
    -webkit-transition: 0.5s ease-in-out;
    -o-transition: 0.5s ease-in-out;
    transition: 0.5s ease-in-out;
}

.dsn-nav-bar.nav-bg>.header-top>.header-container,
.dsn-nav-bar.nav-bg .site-header {
    padding-bottom: 15px;
    padding-top: 15px;
    background-color: #000;
}

.dsn-nav-bar {
    position: absolute;
    z-index: 999;
    width: 100%;
}

.dsn-nav-bar .icon-m {
    overflow: hidden;
    will-change: transform;
}


.dsn-nav-bar .icon-m .menu-icon-close {
    opacity: 0;
    visibility: hidden;
    will-change: transform;
    -webkit-transform: translateY(50%) rotate(15deg) scale(0.8);
    -ms-transform: translateY(50%) rotate(15deg) scale(0.8);
    transform: translateY(50%) rotate(15deg) scale(0.8);
    -webkit-transform-origin: top left;
    -ms-transform-origin: top left;
    transform-origin: top left;
}

.dsn-nav-bar .dsn-wrapper {
    margin-right: 7px;
}

.dsn-nav-bar .dsn-wrapper:last-child {
    margin-right: 0;
}

.dsn-nav-bar .icon-m {
    will-change: transform;
}

.dsn-nav-bar .icon-m .menu-icon__line {
    will-change: transform;
    opacity: 1;
    visibility: visible;
    -webkit-transform: none;
    -ms-transform: none;
    transform: none;
    -webkit-transition: -webkit-transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36);
    transition: -webkit-transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36);
    -o-transition: transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36);
    transition: transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36);
    transition: transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36), -webkit-transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36);
}


.dsn-nav-bar .icon-m:nth-of-type(0) .menu-icon__line {
    -webkit-transition: opacity 0.3s cubic-bezier(0.31, 1.37, 0.68, -0.36) 200ms, visibility 0.3s 0ms, -webkit-transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36) 0ms;
    transition: opacity 0.3s cubic-bezier(0.31, 1.37, 0.68, -0.36) 200ms, visibility 0.3s 0ms, -webkit-transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36) 0ms;
    -o-transition: transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36) 0ms, opacity 0.3s cubic-bezier(0.31, 1.37, 0.68, -0.36) 200ms, visibility 0.3s 0ms;
    transition: transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36) 0ms, opacity 0.3s cubic-bezier(0.31, 1.37, 0.68, -0.36) 200ms, visibility 0.3s 0ms;
    transition: transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36) 0ms, opacity 0.3s cubic-bezier(0.31, 1.37, 0.68, -0.36) 200ms, visibility 0.3s 0ms, -webkit-transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36) 0ms;
}

.dsn-nav-bar .icon-m:nth-of-type(1) .menu-icon__line {
    -webkit-transition: opacity 0.3s cubic-bezier(0.31, 1.37, 0.68, -0.36) 209ms, visibility 0.3s 45ms, -webkit-transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36) 9ms;
    transition: opacity 0.3s cubic-bezier(0.31, 1.37, 0.68, -0.36) 209ms, visibility 0.3s 45ms, -webkit-transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36) 9ms;
    -o-transition: transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36) 9ms, opacity 0.3s cubic-bezier(0.31, 1.37, 0.68, -0.36) 209ms, visibility 0.3s 45ms;
    transition: transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36) 9ms, opacity 0.3s cubic-bezier(0.31, 1.37, 0.68, -0.36) 209ms, visibility 0.3s 45ms;
    transition: transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36) 9ms, opacity 0.3s cubic-bezier(0.31, 1.37, 0.68, -0.36) 209ms, visibility 0.3s 45ms, -webkit-transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36) 9ms;
}

.dsn-nav-bar .icon-m:nth-of-type(2) .menu-icon__line {
    -webkit-transition: opacity 0.3s cubic-bezier(0.31, 1.37, 0.68, -0.36) 218ms, visibility 0.3s 90ms, -webkit-transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36) 18ms;
    transition: opacity 0.3s cubic-bezier(0.31, 1.37, 0.68, -0.36) 218ms, visibility 0.3s 90ms, -webkit-transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36) 18ms;
    -o-transition: transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36) 18ms, opacity 0.3s cubic-bezier(0.31, 1.37, 0.68, -0.36) 218ms, visibility 0.3s 90ms;
    transition: transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36) 18ms, opacity 0.3s cubic-bezier(0.31, 1.37, 0.68, -0.36) 218ms, visibility 0.3s 90ms;
    transition: transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36) 18ms, opacity 0.3s cubic-bezier(0.31, 1.37, 0.68, -0.36) 218ms, visibility 0.3s 90ms, -webkit-transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36) 18ms;
}

.dsn-nav-bar .icon-m:nth-of-type(3) .menu-icon__line {
    -webkit-transition: opacity 0.3s cubic-bezier(0.31, 1.37, 0.68, -0.36) 227ms, visibility 0.3s 135ms, -webkit-transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36) 27ms;
    transition: opacity 0.3s cubic-bezier(0.31, 1.37, 0.68, -0.36) 227ms, visibility 0.3s 135ms, -webkit-transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36) 27ms;
    -o-transition: transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36) 27ms, opacity 0.3s cubic-bezier(0.31, 1.37, 0.68, -0.36) 227ms, visibility 0.3s 135ms;
    transition: transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36) 27ms, opacity 0.3s cubic-bezier(0.31, 1.37, 0.68, -0.36) 227ms, visibility 0.3s 135ms;
    transition: transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36) 27ms, opacity 0.3s cubic-bezier(0.31, 1.37, 0.68, -0.36) 227ms, visibility 0.3s 135ms, -webkit-transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36) 27ms;
}

body.nav-active .dsn-nav-bar .dsn-wrapper {
    margin-right: 7px;
}

body.nav-active .dsn-nav-bar .dsn-wrapper:last-child {
    margin-right: 0;
}



body.nav-active .dsn-nav-bar .icon-m {
    will-change: transform;
}

body.nav-active .dsn-nav-bar .icon-m .menu-icon-close {
    will-change: transform;
    opacity: 1;
    visibility: visible;
    -webkit-transform: none;
    -ms-transform: none;
    transform: none;
    -webkit-transition: -webkit-transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36);
    transition: -webkit-transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36);
    -o-transition: transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36);
    transition: transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36);
    transition: transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36), -webkit-transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36);
}

body.nav-active .dsn-nav-bar .icon-m:nth-of-type(0) .menu-icon-close {
    -webkit-transition: opacity 0.3s cubic-bezier(0.31, 1.37, 0.68, -0.36) 1200ms, visibility 0.3s 1000ms, -webkit-transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36) 1000ms;
    transition: opacity 0.3s cubic-bezier(0.31, 1.37, 0.68, -0.36) 1200ms, visibility 0.3s 1000ms, -webkit-transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36) 1000ms;
    -o-transition: transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36) 1000ms, opacity 0.3s cubic-bezier(0.31, 1.37, 0.68, -0.36) 1200ms, visibility 0.3s 1000ms;
    transition: transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36) 1000ms, opacity 0.3s cubic-bezier(0.31, 1.37, 0.68, -0.36) 1200ms, visibility 0.3s 1000ms;
    transition: transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36) 1000ms, opacity 0.3s cubic-bezier(0.31, 1.37, 0.68, -0.36) 1200ms, visibility 0.3s 1000ms, -webkit-transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36) 1000ms;
}

body.nav-active .dsn-nav-bar .icon-m:nth-of-type(1) .menu-icon-close {
    -webkit-transition: opacity 0.3s cubic-bezier(0.31, 1.37, 0.68, -0.36) 1209ms, visibility 0.3s 1045ms, -webkit-transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36) 1009ms;
    transition: opacity 0.3s cubic-bezier(0.31, 1.37, 0.68, -0.36) 1209ms, visibility 0.3s 1045ms, -webkit-transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36) 1009ms;
    -o-transition: transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36) 1009ms, opacity 0.3s cubic-bezier(0.31, 1.37, 0.68, -0.36) 1209ms, visibility 0.3s 1045ms;
    transition: transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36) 1009ms, opacity 0.3s cubic-bezier(0.31, 1.37, 0.68, -0.36) 1209ms, visibility 0.3s 1045ms;
    transition: transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36) 1009ms, opacity 0.3s cubic-bezier(0.31, 1.37, 0.68, -0.36) 1209ms, visibility 0.3s 1045ms, -webkit-transform 0.5s cubic-bezier(0.31, 1.37, 0.68, -0.36) 1009ms;
}

body.nav-active .dsn-nav-bar .icon-m {
    overflow: hidden;
    will-change: transform;
}

body.nav-active .dsn-nav-bar .icon-m .menu-icon__line {
    opacity: 0;
    visibility: hidden;
    will-change: transform;
    -webkit-transform: translateY(50%) rotate(15deg) scale(0.8);
    -ms-transform: translateY(50%) rotate(15deg) scale(0.8);
    transform: translateY(50%) rotate(15deg) scale(0.8);
    -webkit-transform-origin: top left;
    -ms-transform-origin: top left;
    transform-origin: top left;
}
</style>