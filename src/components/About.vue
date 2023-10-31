<template>
    <div class="about container align-items-center" id="about">
        <div class="square-1" :style="{ transform: `translateX(${dinamicLeftSquare}px)` }"></div>
        <div class="square-2" :style="{ transform: `translateY(${dinamicLeftSquare}px)` }"></div>
        <div class="square-3" :style="{ transform: `translateX(${dinamicRightSquare}px)` }"></div>
        <div class="square-4" :style="{ transform: `translateX(${dinamicRightSquare}px)` }"></div>
        <div class="row">
            <div class="offset-md-3 col-md-4">
                <span class="title d-block">About Me</span>
                <h1>I'm <span class="title">Nizar</span></h1>
                <span>I am a Front End Developer with 2 - 3 years of
                    experience, and I'm very passionate and dedicated to my work.
                    <br><br>
                    currently working as a Front End
                    Web Developer. I have worked with small and
                    big teams to develop websites and maintain
                    good communication between team
                    members</span>
                <br>
            </div>
        </div>
        <img src="../assets/me.jpg" alt="img" class="img-about">
    </div>
</template>
<script setup>
import { ref, onMounted, onUnmounted } from "vue";

const dinamicLeftSquare = ref(7.20001);
const dinamicRightSquare = ref(7.20001);


const updateScrollY = () => {
    if (window.scrollY > 500 && window.scrollY < 600) {
        dinamicLeftSquare.value = window.scrollY - 500
    }
    if (window.scrollY > 750 && window.scrollY < 850) {
        dinamicRightSquare.value = window.scrollY - 750
    }
};

// Add a scroll event listener when the component is mounted
onMounted(() => {
    window.addEventListener("scroll", updateScrollY);
});

// Remove the scroll event listener when the component is unmounted
onUnmounted(() => {
    window.removeEventListener("scroll", updateScrollY);
});
</script>

<style scoped>
.about {
    position: relative;
    height: 700px;
}

.square-1 {
    transition: transform 3s cubic-bezier(0, 0, 0, 1) 0s;
    position: absolute;
    border: 5px solid white;
    width: 250px;
    height: 250px;
    z-index: 2;
    top: 60px;
    left: -200px;
}

.square-2 {
    transition: transform 3s cubic-bezier(0, 0, 0, 1) 0s;
    left: -50px;
    top: 150px;
    position: absolute;
    background-color: #ffc400cc;
    width: 250px;
    height: 250px;
}

.square-3 {
    transition: transform 3s cubic-bezier(0, 0, 0, 1) 0s;
    right: 0;
    bottom: 80px;
    position: absolute;
    background-color: #ffc400cc;
    width: 300px;
    height: 250px;
}

.square-4 {
    transition: transform 3s cubic-bezier(0, 0, 0, 1) 0s;
    position: absolute;
    border: 5px solid white;
    width: 300px;
    height: 250px;
    z-index: 3;
    right: -100px;
    bottom: -180px;
}


button {
    margin-top: 20px;
    border-radius: 5px;
    transition: all 0.5s ease;
    background-color: #ffc400cc;
    color: #ffff;
    border: none;
    padding: 8px 13px;
}

button:hover {
    background-color: #ffc400;
}

.img-about {
    position: absolute;
    top: 50px;
    width: 400px;
    margin-top: 200px;
    border-radius: 50px;
    right: 30px;
    filter: grayscale(100%);
    z-index: 2;
}

@media (max-width: 900px) {

    .square-1,
    .square-2,
    .square-3,
    .square-4 {
        display: none;
    }

    .img-about {
        position: relative;
        width: 250px;
        margin: 0;
        display: block;
        margin-left: auto;
    }

}</style>