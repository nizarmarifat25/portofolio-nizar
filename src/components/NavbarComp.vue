<template>
    <nav class="navbar navbar-expand-lg mx-auto">
        <div class="container">
            <a class="navbar-brand" href="#">Nizar Marifat.</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse"
                data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false"
                aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarSupportedContent">
                <ul class="navbar-nav ms-auto mb-2 mb-lg-0 ">
                    <li class="nav-item">
                        <a class="nav-link" href="#about">About</a>
                    </li>
                    <li class="nav-item ">
                        <a class="nav-link" href="#experience">Experience</a>
                    </li>
                    <li class="nav-item ">
                        <a class="nav-link" href="#projects">Projects</a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>
</template>

<script>
export default {

}
</script>

<style scoped>
.navbar {
    z-index: 99;
    position: fixed;
    left: 0;
    right: 0;
    padding: 20px;
    /* background-color: rgba(2, 27, 56, 1); */
    backdrop-filter: blur(3px);
    background: hsla(2, 27, 56, 1);
    border-bottom: 1px solid rgba(255, 255, 255, 0.171);

}

.nav-link,
.navbar-brand {
    color: white !important;
}

.logo h3 {
    font-weight: bold;
}
</style>