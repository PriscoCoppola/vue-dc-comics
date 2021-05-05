<template>
    <div class="hero">
        <div class="image">
            <img :src="hero.thumb" alt="">
        </div>
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

<style scoped lang="scss">
.hero {
    flex-basis: calc(100% / 6);
    padding: 30px 0;

    .image {
    height: 200px;
    overflow: hidden;
    }

    .text {
    padding-top: 15px;
    color: #fff;
    text-transform: uppercase;
    font-size: 12px;
    }
}
</style>