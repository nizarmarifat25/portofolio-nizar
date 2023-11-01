<template>
    <div class="experience p-5" id="experience">
        <h1 class="">Experience </h1>
        <div class="container">
            <section class="design-section">
                <div class="timeline">
                    <div class="timeline-component timeline-content" data-aos="fade-up" data-aos-duration="2000">
                        <h4>Jr Frontend</h4>
                        <small class="text-secondary">Jun 2021 - Sep 2021</small>
                        <br>
                        <strong>Socket Space </strong> |
                        <small>PT Trasnformasi Data Indonesia</small>
                        <small>
                            <ul>
                                <li>Develop website using Bootstrap framework</li>
                            </ul>
                        </small>
                    </div>
                    <div class="timeline-middle" data-aos="fade-up" data-aos-duration="1500">
                        <div class="timeline-circle"></div>
                    </div>
                    <div class="timeline-empty">
                    </div>
                    <div class="timeline-component timeline-content" data-aos="fade-up" data-aos-duration="2000">
                        <h4>Frontend Developer</h4>
                        <small class="text-secondary">Sep 2021 - Jun 2022</small>
                        <br>
                        <strong>Socket Space </strong> |
                        <small>PT Trasnformasi Data Indonesia</small>
                        <small>
                            <ul>
                                <li>Develop website using React Js framework</li>
                                <li>Design and implement solutions for user needs (web)</li>
                                <li>Collaborate with Backend Team for API integration</li>
                            </ul>
                        </small>
                    </div>
                    <div class="timeline-middle" data-aos="fade-up" data-aos-duration="500">
                        <div class="timeline-circle"></div>
                    </div>
                    <div class="timeline-empty">
                    </div>
                    <div class="timeline-component timeline-content" data-aos="fade-up" data-aos-duration="2000">
                        <h4>Web Software Engineer</h4>
                        <small class="text-secondary">Aug 2022 - Present</small>
                        <br>
                        <strong>ICON+ </strong> |
                        <small>PT Indonesia comnets plus</small>
                        <small>
                            <ul>
                                <li>Web Maintenance and Development</li>
                                <li>designing web and mobile applications (UI/UX)</li>
                                <li>Create Web Applications and develop using Vue js , NEXT JS and NUXT JS</li>
                                <li>Create REST API using ExpressJS Framework</li>
                            </ul>
                        </small>
                    </div>
                    <div class="timeline-middle" data-aos="fade-up" data-aos-duration="500">
                        <div class="timeline-circle"></div>
                    </div>
                    <div class="timeline-empty">
                    </div>
                    <div class="timeline-empty">
                    </div>
                    <div class="timeline-middle" data-aos="fade-up" data-aos-duration="500">
                        <div class="timeline-circle"></div>
                    </div>
                </div>
            </section>
        </div>
    </div>
    <svg id="wave" style="transform:rotate(180deg); transition: 0.3s" viewBox="0 0 1440 100" version="1.1"
        xmlns="http://www.w3.org/2000/svg">
        <defs>
            <linearGradient id="sw-gradient-0" x1="0" x2="0" y1="1" y2="0">
                <stop stop-color="rgba(255, 196, 0, 0.8)" offset="0%"></stop>
                <stop stop-color="rgba(255, 196, 0, 0.8)" offset="100%"></stop>
            </linearGradient>
        </defs>
        <path style="transform:translate(0, 0px); opacity:1" fill="url(#sw-gradient-0)"
            d="M0,50L60,90L120,90L180,30L240,50L300,70L360,30L420,30L480,10L540,10L600,30L660,70L720,30L780,80L840,40L900,20L960,80L1020,40L1080,60L1140,30L1200,0L1260,0L1320,0L1380,30L1440,50L1440,100L1380,100L1320,100L1260,100L1200,100L1140,100L1080,100L1020,100L960,100L900,100L840,100L780,100L720,100L660,100L600,100L540,100L480,100L420,100L360,100L300,100L240,100L180,100L120,100L60,100L0,100Z">
        </path>
    </svg>
</template>

<style>
.experience {
    position: relative;
    background-color: #ffc400cc;
}

.experience h1 {
    position: absolute;
    right: 150px;
    top: 350px;
    font-size: 50px;

}

.timeline {
    width: 80%;
    height: auto;
    max-width: 900px;
    display: flex;
    flex-direction: column;
}

.timeline-content {
    padding: 20px;
    background: #ffff;
    border-radius: 5px;
    color: black;
    padding: 1.75rem;
    transition: 0.4s ease;
    overflow-wrap: break-word !important;
    margin: 1rem;
    margin-bottom: 20px;
    border-radius: 6px;
}

.timeline-component h4 {
    font-weight: 1000;
    color: #ffc400;
}

.timeline-component {
    margin: 0px 20px 20px 20px;
}


@media screen and (min-width: 768px) {
    .timeline {
        display: grid;
        grid-template-columns: 1fr 3px 1fr;
    }

    .timeline-middle {
        position: relative;
        background-color: #ffff;
        width: 3px;
        height: 100%;
    }

    .main-middle {
        opacity: 0;
    }

    .timeline-circle {
        position: absolute;
        top: 0;
        left: 50%;
        width: 15px;
        height: 15px;
        border-radius: 50%;
        background-color: #fff;
        -webkit-transform: translateX(-50%);
        transform: translateX(-50%);
    }
}

@media (max-width: 900px) {
    .experience h1 {
        top: 20px;
        right: 0;
        position: relative;
    }

    .timeline-component {
        margin: 10px 0;
    }
    .timeline {
        width: 100%;
    }
    .timeline {
        margin-top: 50px;
    }
}

@media (max-width: 420px) {
    .experience h1 {
        top: 80px;
        right: 0;
        position: relative;
    }

    .timeline {
        margin-top: 100px;
    }
}
</style>