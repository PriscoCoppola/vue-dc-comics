<template>
    <footer>
        <div class="footer-top">
            <div class="container">
                <div class="links">
                    <div class="m-right">
                        <h2>Dc Comics</h2>
                        <ul>
                            <li
                                v-for="(link, index) in dcComics"
                                :key="index"
                            >
                                <a :href="link.url">{{ link.name }}</a>
                            </li>
                        </ul>
                        <h2>Shop</h2>
                        <ul>
                            <li
                                v-for="(link, index) in shop"
                                :key="index"
                            >
                                <a :href="link.url">{{ link.name }}</a>
                            </li>
                        </ul>
                    </div>
                    <div class="m-right">
                        <h2>DC</h2>
                        <ul>
                            <li
                                v-for="(link, index) in dc"
                                :key="index"
                            >
                                <a :href="link.url">{{ link.name }}</a>
                            </li>
                        </ul>
                    </div>
                    <div class="m-right">
                        <h2>Sites</h2>
                        <ul>
                            <li
                                v-for="(link, index) in sites"
                                :key="index"
                            >
                                <a :href="link.url">{{ link.name }}</a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="logo">
                    <img src="../assets/images/dc-logo-bg.png" alt="Logo BG">
                </div>
            </div>
        </div>
        <div class="footer-bottom">
            <div class="container">
                <div class="button">
                    Sign-up now!
                </div>

                <div class="social">
                    <h2 class="blue">follow us</h2>
                    <img src="../assets/images/footer-facebook.png" alt="">
                    <img src="../assets/images/footer-twitter.png" alt="">
                    <img src="../assets/images/footer-youtube.png" alt="">
                    <img src="../assets/images/footer-pinterest.png" alt="">
                    <img src="../assets/images/footer-periscope.png" alt="">
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'Footer',
    data() {
        return {
            dcComics: [
                {
                    name: 'Characters',
                    url: '/characters',
                },
                {
                    name: 'Comics',
                    url: '/comics',
                },
                {
                    name: 'Movies',
                    url: '/movies',
                },
                {
                    name: 'TV',
                    url: '/tv',
                },
                {
                    name: 'Games',
                    url: '/games',
                },
                {
                    name: 'Videos',
                    url: '/videos',
                },
                {
                    name: 'News',
                    url: '/news',
                },
            ],
            shop: [
                {
                    name: 'Shop DC',
                    url: '/shopdc',
                },
                {
                    name: 'Shop DC Collectibles',
                    url: '/shopdccollectibles',
                },
            ],
            dc: [
                {
                    name: 'Terms Of Use',
                    url: '/termsofuse',
                },
                {
                    name: 'Privacy policy (New)',
                    url: '/privacypolicy',
                },
                {
                    name: 'Ad Choices',
                    url: '/adchoices',
                },
                {
                    name: 'Advertising',
                    url: '/advertising',
                },
                {
                    name: 'Jobs',
                    url: '/jobs',
                },
                {
                    name: 'Subscriptions',
                    url: '/subscriptions',
                },
                {
                    name: 'Talent Workshops',
                    url: '/talentworkshops',
                },
                {
                    name: 'CPSC Certificates',
                    url: '/cpsccertificates',
                },
                {
                    name: 'Ratings',
                    url: '/ratings',
                },
                {
                    name: 'Shop Help',
                    url: '/shophelp',
                },
                {
                    name: 'Contact Us',
                    url: '/contactus',
                },
            ],
            sites: [
                {
                    name: 'DC',
                    url: '/dc',
                },
                {
                    name: 'MAD Magazine',
                    url: '/madmagazine',
                },
                {
                    name: 'DC Kids',
                    url: '/dckids',
                },
                {
                    name: 'DC Universe',
                    url: '/dcuniverse',
                },
                {
                    name: 'DC Power Visa',
                    url: '/dcpowervisa',
                },
            ],
        }
    }
}
</script>

<style scoped>
.footer-top {
    background-image: url(../assets/images/footer-bg.jpg);
}

.container {
    display: flex;
    justify-content: space-between;
    width: 1200px;
    margin: 0 auto;
    padding: 2rem 0;
    overflow: hidden;
}

.links {
    display: flex;
}

.logo {
    height: 280px;
}

.logo img {
    transform: translateY(-127px)
}

.m-right {
    margin-right: 2rem;
}

h2 {
    text-transform: uppercase;
    font-weight: bold;
    color: #fff;
}

ul {
    padding: 1rem 0;
    list-style: none;
}

ul li a {
    text-decoration: none;
    color: #959595;
    line-height: 22px;
    font-size: 14px;
}

.footer-bottom {
    background-color: #303030
}

.button {
    border: 3px solid #0282f9;
    color: #fff;
    text-transform: uppercase;
    font-size: 22px;
    height: 55px;
    padding: 15px;
    cursor: pointer;
}

.blue {
    color: #0282f9;
    margin-right: 20px;
}

.social {
    display: flex;
    align-items: center;
}

.footer-bottom img {
    padding: 10px;
    cursor: pointer;
}
</style>