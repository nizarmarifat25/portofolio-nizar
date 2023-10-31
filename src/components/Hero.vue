<template>
        <div class="container hero">
            <div class="row d-flex align-items-center h-100">
                <div class="col align-items-center">
                    <h3><span class="title">Hi</span>, I'm Nizar</h3>
                    <h2 class="text-muted text-center">Web Developer | Frontend</h2>
                </div>
            </div>
        </div>
        <div id="particles-js"></div>
</template>
    
<script>
import 'particles.js'
export default {
    name: 'hero',
    mounted() {
        this.initParticles()
    },
    methods: {
        initParticles() {
            window.particlesJS("particles-js", {
                "particles": {
                    "number": {
                        "value": 200,
                        "density": {
                            "enable": true,
                            "value_area": 900
                        }
                    },
                    "color": {
                        "value": "#ffffff"
                    },
                    "shape": {
                        "type": "circle",
                        "stroke": {
                            "width": 0,
                            "color": "#000000"
                        },
                        "polygon": {
                            "nb_sides": 5
                        },
                    },
                    "opacity": {
                        "value": 0.5,
                        "random": false,
                        "anim": {
                            "enable": false,
                            "speed": 1,
                            "opacity_min": 0.1,
                            "sync": false
                        }
                    },
                    "size": {
                        "value": 3,
                        "random": true,
                        "anim": {
                            "enable": false,
                            "speed": 40,
                            "size_min": 0.1,
                            "sync": false
                        }
                    },
                    "line_linked": {
                        "enable": true,
                        "distance": 150,
                        "color": "#ffffff",
                        "opacity": 0.4,
                        "width": 1
                    },
                    "move": {
                        "enable": true,
                        "speed": 6,
                        "direction": "none",
                        "random": false,
                        "straight": false,
                        "out_mode": "out",
                        "bounce": false,
                        "attract": {
                            "enable": false,
                            "rotateX": 600,
                            "rotateY": 1200
                        }
                    }
                },
                "interactivity": {
                    "detect_on": "canvas",
                    "events": {
                        "onhover": {
                            "enable": true,
                            "mode": "grab"
                        },
                        "onclick": {
                            "enable": true,
                            "mode": "push"
                        },
                        "resize": true
                    },
                    "modes": {
                        "grab": {
                            "distance": 140,
                            "line_linked": {
                                "opacity": 1
                            }
                        },
                        "bubble": {
                            "distance": 400,
                            "size": 40,
                            "duration": 2,
                            "opacity": 8,
                            "speed": 3
                        },
                        "repulse": {
                            "distance": 200,
                            "duration": 0.4
                        },
                        "push": {
                            "particles_nb": 4
                        },
                        "remove": {
                            "particles_nb": 2
                        }
                    }
                },
                "retina_detect": true
            })
        }
    }
}
</script>
    
<style  scoped>
.hero {
    align-items: center;
    height: 100vh;
}

h3 {
    text-align: center;
    font-size: 100px;
    font-weight: bold;
}
#particles-js {
    margin-top: -100vh;
    z-index: -100;
    height: 100vh !important;
    
}
@media (max-width: 720px) {
    h3{
        font-size: 50px;
    }
}
</style>