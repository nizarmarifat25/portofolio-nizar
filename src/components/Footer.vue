<template>
    <footer>
        <div className="art text-center mt-4">
            <div class="container">
                <p className="text-white">Kp. Lame, Desa Mekarsari, Kec. Selaawi, Kab.Garut, Provinsi Jawa Barat</p>
                <p className="text-white">Follow Me On :</p>
                <a className="btn-floating text-dark" href="https://www.instagram.com/nizarmarifat/" target="_blank">
                    <i className="fab fa-instagram">
                        <img src="../assets/img/ig.svg" style="width: 16px;"  alt="">

                    </i>
                </a>
                <a className="btn-floating text-dark" href="https://www.linkedin.com/in/nizar-marifat/" target="_blank">
                    <i className="fab fa-linkedin">
                        <img src="../assets/img/linkdin.svg" style="width: 16px;" alt="">
                    </i>
                </a>
                <p className="text-white">Contact Me | <span className="text-dark">+6282258766060</span></p>
            </div>
        </div>
    </footer>
</template>
<style>
footer {
    margin-top: 80px;
    background-color: #003049;
    line-height: 24px;
    font-family: Arial, Helvetica, sans-serif;
}

footer .art {
    background: #ffc400cc;
    padding-bottom: 30px;
    padding-top: 48px;
    clip-path: polygon(0% 5%, 15% 0%, 100% 10%, 100% 100%, 0% 100%);
}

footer .art a {
    text-decoration: none;
}

footer .content {
    max-width: 1080px;
    margin: auto;
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-gap: 16px;
}

footer .social {
    display: grid;
    grid-template-columns: repeat(5, 1fr);
    grid-gap: 16px;
}

footer i {
    font-size: 32px;
    padding: 0 10px;
    text-align: center;
}

footer i:hover {
    color: #fff;
}

footer p {
    font-size: 15px;
    font-weight: 300;
    margin: 5px 0;
}

footer .notice {
    text-align: center;
    color: #fff;
}
</style>