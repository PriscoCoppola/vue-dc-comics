<template>
    <section>
        <div class="container">
            <ul>
                <li
                    v-for="(link, index) in links"
                    :key="index"
                >
                    <img src="../assets/images/buy-comics-digital-comics.png" :alt="link.name">
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
                    image: 'buy-comics-digital-comics'
                },
                {
                    name: 'DC Merchandise',
                    url: '/dcmerchandise',
                    image: 'buy-comics-merchandise'
                },
                {
                    name: 'Subscription',
                    url: '/subscription',
                    image: 'buy-comics-subscriptions'
                },
                {
                    name: 'Comic Shop Locator',
                    url: '/comicshoplocator',
                    image: 'buy-comics-shop-locator'
                },
                {
                    name: 'DC Power Visa',
                    url: '/dcpowervisa',
                    image: 'buy-dc-power-visa'
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
    width: 35px;
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