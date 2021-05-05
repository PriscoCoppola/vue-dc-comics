<template>
    <section>
        <div class="container">
            <ul>
                <li
                    v-for="(link, index) in links"
                    :key="index"
                >
                    <img :src="link.image" :alt="link.name">
                    <a :href="link.url">{{link.name}}</a>
                </li>
            </ul>
        </div>
    </section>
</template>

<script>
export default {
    name: 'Products',
    data() {
        return {
            links: [
                {
                    name: 'Digital Comics',
                    url: '/digitalcomics',
                    image:require('../assets/images/buy-comics-digital-comics.png'),
                },
                {
                    name: 'DC Merchandise',
                    url: '/dcmerchandise',
                    image:require('../assets/images/buy-comics-merchandise.png'),
                },
                {
                    name: 'Subscription',
                    url: '/subscription',
                    image:require('../assets/images/buy-comics-subscriptions.png'),
                },
                {
                    name: 'Comic Shop Locator',
                    url: '/comicshoplocator',
                    image:require('../assets/images/buy-comics-shop-locator.png'),
                },
                {
                    name: 'DC Power Visa',
                    url: '/dcpowervisa',
                    image:require('../assets/images/buy-dc-power-visa.svg'),
                },
            ],
        }
    }
}
</script>

<style scoped>
section {
    background-color: #0282f9
}

.container {
    width: 1200px;
    margin: 0 auto;
}

ul {
    display: flex;
    justify-content: center;
}

li {
    display: flex;
    align-items: center;
    padding: 3rem;
    list-style: none;
}

li img {
    width: 50px;
    color: #fff;
}

li a {
    padding-left: 10px;
    text-decoration: none;
    text-transform: uppercase;
    color: #fff;
    font-size: 12px;
}
</style>