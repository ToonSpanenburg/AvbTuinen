<script setup>

</script>

<template>
    <div v-if="windowWidth > 800">
        <div class="row m-4 align-items-center ">
            <div class="col-6 ms-3">
                <img src="/logo.jpg" alt="">
            </div>
            <div class="col text-center">
                <a class="" href="">
                    Home
                </a>
            </div>
            <div class="col text-center">
                <a href="">Introductie</a>
            </div>
            <div class="col text-center">
                <a href="">Diensten</a>
            </div>
            <div class="col text-center">
                <a href="">Contact</a>
            </div>
        </div>
    </div>
    <div v-else>
        <nav class="navbar bg-white fixed-top p-2">
            <div class="container-fluid">

                <img src="/logo.jpg" alt="">
                <button class="navbar-toggler" type="button" data-bs-toggle="offcanvas" data-bs-target="#mobileNav" aria-controls="mobileNav" aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                </button>

                <div class="offcanvas offcanvas-end " tabindex="-1" id="mobileNav" aria-labelledby="offcanvasDarkNavbarLabel">
                    <div class="offcanvas-header">
                        <h5 class="offcanvas-title" id="offcanvasDarkNavbarLabel">Avb Tuinen</h5>
                        <button type="button" class="btn-close btn-close-white" data-bs-dismiss="offcanvas" aria-label="Close"></button>
                    </div>
                    <div class="offcanvas-body">
                        <ul class="navbar-nav justify-content-end flex-grow-1 pe-3">
                            <li class="nav-item">
                                <a class="nav-link active" aria-current="page" href="#">Home</a>
                            </li>
                            <li class="nav-item">
                                <a class="nav-link" href="#">Link</a>
                            </li>

                        </ul>
                    </div>
                </div>
            </div>
        </nav>
    </div>
</template>

<script>
export default {
    data() {
        return {
            windowWidth: window.innerWidth,
        };
    },
    mounted() {
        window.addEventListener('resize', this.handleResize);
    },
    beforeDestroy() {
        window.removeEventListener('resize', this.handleResize);
    },
    methods: {
        handleResize() {
            this.windowWidth = window.innerWidth;
        },
    },
};
</script>

<style scoped>
img
{
  height: 3em;
}
a
{
  font-family: Baskerville Serif;
  color: black;
  text-decoration: none;
}
a:hover
{
  text-decoration: underline black solid ;
}

@media (min-width: 992px) {
    a {
        font-size: 1.6em;
    }
}
@media (min-width: 1200px) {
    a {
        font-size: 2em;
    }
}
</style>