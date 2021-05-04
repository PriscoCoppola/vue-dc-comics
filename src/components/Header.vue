<template>
    <header>
        <img src="../assets/images/dc-logo.png" alt="Logo">

        <ul>
            <li 
                v-for="(link, index) in links" 
                :key="index"
            >
                <a
                    :href="link.url"
                    :class="{ active: link.active === true }"
                >
                    {{ link.name }}
                </a>
            </li>
        </ul>
    </header>
</template>

<script>
export default {
    name: 'Header',
    data() {
        return {
            links: [
                {
                    name: 'Characters',
                    url: '/characters',
                    active: false
                },
                {
                    name: 'Comics',
                    url: '/comics',
                    active: true
                },
                {
                    name: 'Movies',
                    url: '/movies',
                    active: false
                },
                {
                    name: 'Tv',
                    url: '/tv',
                    active: false
                },
                {
                    name: 'Games',
                    url: '/games',
                    active: false
                },
                {
                    name: 'Collectibles',
                    url: '/collectibles',
                    active: false
                },
                {
                    name: 'Videos',
                    url: '/videos',
                    active: false
                },
                {
                    name: 'Fans',
                    url: '/fans',
                    active: false
                },
                {
                    name: 'News',
                    url: '/news',
                    active: false
                },
                {
                    name: 'Shop',
                    url: '/shop',
                    active: false
                },
            ],  
        }
    },
}
</script>

<style scoped>
header {
    max-width: 1200px;
    margin: 0 auto;
    padding: 1rem 0;
    display: flex;
    justify-content: space-between;
    font-size: 12px;
}

img {
    width: 75px;
}

ul {
    display: flex;
    align-items: center;
    list-style: none;
}

li {
    padding: 0 1rem;
}

li a {
    padding: 42px 0;
    text-decoration: none;
    text-transform: uppercase;
    color: #000;
    font-weight: bold;
}

li a:hover,
li a.active {
    color: #0282f9;
    border-bottom: 5px solid #0282f9;
}
</style>