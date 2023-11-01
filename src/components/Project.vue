<template>
    <div class="container">
        <h1 class="mt-3">PROJECT</h1>
        <div id="projects">
            <div class="row justify-content-center">
                <div class="col-md-4 my-3" v-for="(data, i ) in dataProject" :key="i">
                    <div class="card card-1" data-bs-toggle="modal" data-bs-target="#exampleModal" data-aos="fade-up"
                        data-aos-duration="1000" @click="handleDetail(data)">
                        <img :src="data.img" class="w-100" alt="">
                    </div>
                </div>
            </div>
        </div>
    </div>
    <!-- modal -->
    <div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
        <div class="modal-dialog modal-xl modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header">
                    <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                </div>
                <div class="modal-body" style="background-color: #ffc400cc;">
                    <div class="row">
                        <div class="col-md modal-left px-5"  style="color: #003049;">
                            <small class="fw-bolder">as a {{ dataDetail.as_a }}</small>
                            <h4 >{{ dataDetail.title }}</h4>
                            <strong>{{ dataDetail.name }}</strong> <br>
                            <span>Features : </span>
                            <ul >
                                <li v-for="(data, i) in dataDetail.feature" :key="i">{{ data }}</li>
                            </ul>
                            <small v-if="dataDetail.link">click <a :href="dataDetail.link" target="_blank"><i> here</i></a>
                                to visit page</small> <br>
                            <small class="pt-2 mx-1 badge bg-light text-dark" v-for="(data, index) in dataDetail.tech_used"
                                :key="index">{{ data }} </small>
                        </div>
                        <div class="col-md p-5">
                            <img :src="dataDetail.img" alt="" class="w-100  shadow">
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script setup>
import { ref } from 'vue'
import img1 from '../assets/img/project-1.jpeg'
import img2 from '../assets/img/project-2.jpeg'
import img3 from '../assets/img/project-3.jpeg'
import img4 from '../assets/img/project-4.jpeg'
import img5 from '../assets/img/project-5.jpg'
import img6 from '../assets/img/project-6.jpg'
import img7 from '../assets/img/project-7.jpg'

const dataProject = [
    {
        title: 'Arya fire',
        name: 'Strong reminder to replace extinguisher',
        img: img1,
        as_a: 'Fullstack',
        feature: [
            'Notification with audio',
            'Responsive',
            'Export data to excel with filter date',
            'CRUD'
        ],
        tech_used: [
            'PHP',
            'MySQL',
            'Bootstrap'
        ]
    },
    {
        title: 'Zodiak Group',
        name: 'Mining ERP',
        img: img2,
        as_a: 'Frontend',
        feature: [
            'Authentication',
            'Control coal production',
            'Control finances (journals, worksheets, ledgers)',
            'Control the vehicle (service, fuel)',
            'Monitor Revenue, Production and Sales Coal',
            'Export and import data with filter date',
            'etc'
        ],
        tech_used: [
            'ReactJS',
            'Bootstrap',
        ]
    },
    {
        title: 'Wedding Invitation',
        name: 'INVITATION',
        img: img3,
        as_a: 'Frontend',
        feature: [
            'Dinamic comment box',
            'Music on the web',
            'Wedding Day Countdown',
            'Payment gateway QR',
            'Responsive',
        ],
        tech_used: [
            'HTML',
            'CSS',
            'JavaScript',
        ]
    },
    {
        title: 'GEOTOUR BATUR',
        name: 'Company Profile',
        img: img4,
        as_a: 'Frontend',
        link: 'https://geotourbatur.com/#/',
        feature: [
            'Dinamic comment box',
            'Music on the web',
            'Wedding Day Countdown',
            'Payment gateway QR',
            'Responsive',
        ],
        tech_used: [
            'ReactJS',
            'Bootstrap',
        ]
    },
    {
        name: 'Admin Dashboard',
        title: 'NEW ITO',
        img: img5,
        as_a: 'Frontend',
        feature: [
            'Authentication with captcha',
            'Control Customer debt Monitoring',
            'Dinamic menu with Role Login',
            'monitoring work orders, revenue with filter date',
            'Import and Export Data Excel',
            'Tracking workers using leaflet',
            'Responsive',
        ],
        tech_used: [
            'Vue JS',
            'Ant Design',
            'Spring Boot',
            'Oracle Database',
        ]
    },
    {
        name: 'Landing Page',
        title: 'Web Portal Layanan PLN',
        img: img6,
        as_a: 'Frontend',
        feature: [
            'Authentication with captcha',
            'Control Monitoring Customer with multiple filter',
            'Dinamic menu with Role Login',
            'monitor work orders, revenue with filter date',
            'Import and Export Data Excel',
            'Responsive',
        ],
        tech_used: [
            'NUXT JS',
            'Bootstrap',
        ]
    },
    {
        title: 'E-Commerce',
        name: 'nizarpedia',
        img: img7,
        as_a: 'Fullstack',
        feature: [
            'Authentication',
            'Checkout product',
            'Filter Product by category',
            'Cart product',
            'Monitoring Transaction',
        ],
        tech_used: [
            'ReactJS',
            'ExpressJS',
            'MySql',
        ]
    },
]
const dataDetail = ref({})

const handleDetail = (data) => {
    dataDetail.value = data
}
</script>


<style>
.card {
    border-radius: 4px;
    border: 3px solid #ffc300;
    transition: all 0.5s ease;
    cursor: pointer;
}

.card:hover {
    transform: scale(1.05);
}


.modal-left h4 {
    font-size: 30px;
    font-weight: bold;
}

@media (max-width: 900px) {
    .col img {
        display: none;
    }
}
</style>