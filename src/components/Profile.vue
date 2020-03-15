<template>
    <div class="container-fluid px-0 mt-5">
        <article id="home" class="header">
            <section>
                <h2>Welcome to <i>My</i><br>Website!</h2>
                <button class="btn btn-xl btn-dark">Recent Project</button>
            </section>
        </article>
        <article class="profile">
            <section id="profile">
                <div class="container-fluid">
                    <div class="row row-about">
                        <div class="col-md-6 text-center">
                        <img src="../assets/1.png" class="img-about img-fluid m-4">
                        </div>
                        <div class="col-md-6">
                            <h1>About Me</h1>
                            <br/>
                            <p class="text-justify p-4">
                                Nama saya Alif Setyakurniawan, Saya merupakan seorang individu yang terbiasa bersosialisasi, bertemu serta berkerja sama dengan orang baru itu hal biasa bagi saya. Hal menarik dari diri saya adalah sangat dikenal sebagai seorang pendengar yang baik untuk setiap orang yang ada di sekeliling saya.
                                Saya merupakan orang yang dapat mengambil keputusan yang tepat bahkan saat dalam tekanan. Semua pekerjaan yang di serahkan pada saya, pasti akan selalu saya kerjakan dengan detail dan selesai tepat waktu.
                            </p>
                            <br/>
                            <a href="https://www.linkedin.com/in/alif-setyakurniawan-1184721a0/"><button class="btn btn-profile btn-info mb-5">See More</button></a>
                        </div>
                    </div>
                </div>
            </section>
        </article>
        <article id="services" class="blue-section">
            <section class="container">
                <h2>Service</h2>
                <div class="row">
                    <div class="col-lg-3 col-md-6 mb-5 mb-lg-0" v-for="(offers, index) in offers" :key="index">
                        <div class="icon mx-auto"><i class="fas" :class="offers.icon"></i></div>
                        <h4>{{ offers.title }}</h4>
                        <span>{{ offers.description }}</span>
                    </div>
                </div>
            </section>
        </article>
        <article class="education">
            <section id="education">
                <div class="container-fluid container-education">
                    <h1 class="text-center">My Education</h1>
                    <div class="row row-education">
                        <div class="col-md-6" v-for="(data, index) in school" :key="index">
                            <div class="card card-education">
                                <div class="card-body">
                                    <div class="row">
                                        <div class="col-4 text-center">
                                            <img v-bind:src="data.foto" class="img-school img-fluid">
                                        </div>
                                        <div class="col-8">
                                            <h4>{{data.nama}}</h4>
                                            <h6>{{data.ket}}</h6>
                                            <h6>{{data.tahun}}</h6>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </section>
        </article>
        <article class="language">
            <section id="language">
                <div class="container-fluid container-language-md-0">
                    <h1 class="text-center">Pemrograman</h1>
                    <div class="row row-language">
                        <div class="col-md-6" v-for="(data, index) in language" :key="index">
                            <div class="card card-language">
                                <div class="card-body">
                                    <div class="row">
                                        <div class="col-4 text-center">
                                            <img v-bind:src="data.foto" class="img-language img-fluid">
                                        </div>
                                        <div class="col-8">
                                            <h4>{{data.nama}}</h4>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </section>
        </article>
        <article id="find-more" class="white-section">
            <section>
                <h3>Alif Setyakurniawan</h3>
                <span>Freelace people for anywhere project</span>
                <button class="btn btn-xl btn-dark">What I Offer</button>
            </section>
        </article>
        <section id="contact">
            <footer class="footer-contact">
                <div class="row row-contact">
                    <div class="col-md-4">
                    <!-- <img src="../assets/images/logo1.png" alt="logo" class="logo-footer img-fluid"> -->
                        <br/>
                        <p class="link-footer">Official Webpage</p>
                    </div>
                    <div class="col-md-4 pl-4">
                        <p><b>Quick Links</b></p>
                        <div class="row">
                            <div class="col-6">
                                <a href="/" class="link-footer"><p>Home</p></a>
                                <a href="#services" class="link-footer"><p>Services</p></a>
                                <a href="#language" class="link-footer"><p>Language</p></a>
                            </div>
                            <div class="col-6">
                                <a href="#profile" class="link-footer"><p>Profile</p></a>
                                <a href="#education" class="link-footer"><p>Education</p></a>
                                <a href="#contact" class="link-footer"><p>Contact</p></a>
                            </div>
                        </div>
                    </div>
                    <div class="col-md-4">
                        <p><b>Contact Us</b></p>
                        <p class="link-footer">
                    Email : <a href="mailto:alifkurniawan292@gmail.com" class="link-footer">
                        alifkurniawan292@gmail.com</a>
                        </p>
                        <p class="link-footer">
                    WhatsApp: <a href="tel:+6285646023469" class="link-footer">+6285646023469</a>
                        </p>
                        <p class="link-footer">Instagram : <a href="https://www.instagram.com/alifsk_" class="link-footer">@alifsk_</a></p>
                        <p class="link-footer">Twitter : <a href="https://twitter.com/Alifsk_" class="link-footer">@Alifsk_</a></p>
                    </div>
                </div>
                <br/><br/>
                <p class="text-center link-footer">
                    Copyright &copy;2020 Created by <a href="https://www.instagram.com/alifsk_">Alif Setyakurniawan</a>.
                </p>
            </footer>
        </section>
    </div>
</template>

<script>
import ImgSch1 from '../assets/Img1.png';
import ImgSch2 from '../assets/Img2.png';
import ImgSch3 from '../assets/Img3.png';
import ImgSch4 from '../assets/Img4.png';

import b1 from '../assets/b1.png';
import b2 from '../assets/b2.png';
import b3 from '../assets/b3.png';
import b4 from '../assets/b4.png';

export default {
    data: () => {
        return {
            offers: [
                {
                    icon: 'fas fa-laptop-code',
                    title: 'Programmer',
                    description: 'Looks great on any screen size'
                },
                {
                    icon: 'fa-pencil-alt',
                    title: 'Redesigned',
                    description: 'Freshly redesigned for VueJS'
                },
                {
                    icon: 'fas fa-camera-retro',
                    title: 'Photograpy',
                    description: 'Millions of users like us'
                },
                {
                    icon: 'fas fa-address-card',
                    title: 'Biography',
                    description: 'Many People Know Me'
                }
            ],
            school: [
                {
                    id: 1,
                    nama: 'Sekolah Dasar Negeri 1 Pekukuhan',
                    ket: '-',
                    tahun: '2008 - 2013',
                    foto: ImgSch1,
                },
                {
                    id: 2,
                    nama: 'Sekolah Menengah Pertama Negeri 2 Mojosari',
                    ket: '-',
                    tahun: '2013 - 2015',
                    foto: ImgSch2,
                },
                {
                    id: 3,
                    nama: 'Sekolah Menengah Atas Negeri 1 Mojosari',
                    ket: 'Matematika dan Ilmu Pengetahuan Alam',
                    tahun: '2015 - 2018',
                    foto: ImgSch3,
                },
                {
                    id: 4,
                    nama: 'Universitas Brawijaya',
                    ket: 'Pendidikan Vokasi - Sistem Informasi',
                    tahun: '2018 - Present',
                    foto: ImgSch4,
                },
            ],
            language: [
                {
                    id: 1,
                    nama: 'PHP',
                    foto: b1
                },
                {
                    id: 2,
                    nama: 'Java',
                    foto: b2
                },
                {
                    id: 3,
                    nama: 'Android',
                    foto: b3
                },
                {
                    id: 4,
                    nama: 'Python',
                    foto: b4
                },
            ]
        }
    }
}
</script>

<style scoped>
    @import url('https://use.fontawesome.com/releases/v5.8.2/css/all.css');
    @import url('http://stackpath.bootstrapcdn.com/bootstrap/4.2.1/css/bootstrap.min.css');
    @import url('https://fonts.googleapis.com/css?family=Habibi');

    article {
        display: flex;
        justify-content: center;
        align-items: center;
        width: 100%;
        padding: 0 10px;
    }

    .btn-profile {
        padding: 10px 20px;
        font-family: 'Habibi';
        font-size: 1.25rem;
    }

    .btn-xl {
        padding: 20px 35px;
        font-family: 'Habibi';
        font-size: 1.25rem;
    }

    .main-image {
        min-height: 100vh;
        background-size: cover;
        padding: 0 10px;
        text-align: center;
    }

    .header {
        min-height: 100vh;
        background-size: cover;
        padding: 0 10px;
        text-align: center;
        background: url('../assets/table.jpg') center center;
    }

    .profile {
        min-height: 100vh;
        background-size: cover;
        padding: 0 10px;
        text-align: center;
        font-family: 'Habibi';
        background-color: whitesmoke;
    }

    h1 {
        font-size: 5rem;
        font-weight: bold;
        margin-bottom: 30px;
    }

    span {
        display: block;
        padding-bottom: 30px;
        font-size: 1.6rem;
        font-weight: bold;
    }

    .language {
        background-color: #A9A9A9;
    }

    .card-language {
        margin: 20px;
        padding: 10px;
        border: 0;
        border-radius: 0;
        transition: 0.3s ease;
        background-color:#D3D3D3;
        border-radius: 10px;
    }

    .card-language:hover {
        box-shadow:  0px 4px 8px 0px rgba(0, 0, 0, 2);
    }

    .img-language {
        width: 100px;
    }

    .white-section {
        padding: 120px 10px;
        background-color: white;
        text-align: center;
    }

    h3 {
        font-size: 2rem;
        font-weight: bold;
    }

    span {
        display: block;
        padding-bottom: 30px;
        font-size: 1.25rem;
    }

    .blue-section {
        padding: 120px 10px;
        background-color:dodgerblue;
        color: #fff;
        text-align: center;
    }

    h2 {
        font-size: 3rem;
        font-weight: bold;
        margin-bottom: 50px;
    }

    h4 {
        font-size: 1.6rem;
        padding-top: 20px;
    }

    .icon {
        display: flex;
        justify-content: center;
        align-items: center;
        width: 120px;
        height: 120px;
        background-color: white;
        color: dodgerblue;
        border-radius: 50%;
    }

    i {
        font-size: 2rem;
    }

    .container-education, .container-experiences {
        background-color: #f5f5f5;
    }
    .card-education {
        margin: 20px;
        padding: 10px;
        border: 0;
        border-radius: 0;
        transition: 0.3s ease;
    }
    .card-education:hover {
        box-shadow:  0px 4px 8px 0px rgba(0, 0, 0, 2);
    }
    .exp-link {
        text-decoration: none;
    }
    .img-school {
        width: 100px;
    }

    .footer-contact {
        padding: 40px;
        background-color: #141414;
        color: white;
    }
</style>