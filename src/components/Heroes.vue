<template>
    <div class="hero">
        <img :src="hero.thumb" alt="">
        <div class="text">
            {{ hero.series }}
        </div>
    </div>
</template>

<script>
export default {
    name: 'Heroes',
    props: ['hero']
}
</script>

<style scoped>
.hero {
    flex-basis: calc(100% / 6);
    padding: 30px 0;
}

.text {
    padding-top: 15px;
    color: #fff;
    text-transform: uppercase;
    font-size: 12px;
}
</style>