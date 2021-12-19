<template>
    <div>
            <img :src="comic.thumb">
            <span>{{comic.series}}</span>
    </div>
</template>

<script>
export default {
    name: 'MainCards',
    props: {
        comic: Object,
    }
}
</script>

<style lang="scss" scoped>
    @import '../../assets/style/global.scss';

    div {
        width: calc((100% / 6) - 30px);
        margin: 0px 15px 20px;
        display: flex;
        flex-direction: column;
        img {
            width: 100%;
        }
        span {
            margin-top: 5px;
            color: white;
            text-transform: uppercase;
        }
    }
</style>