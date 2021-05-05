<template>
    <div class="album">
        <img :src="album.thumb" alt="album.series">
        <div class="title">{{album.series}}</div>
    </div>
</template>

<script>
export default {
    name: 'Album',
    props: {
        album: Object,
    },

}
</script>

<style scoped lang="scss">
    .album{
        flex-basis: calc(100% / 6 - 28px);
        margin: 0 14px 3rem;
        img{
            width: 100%;
            height: 185px;
            margin-bottom: 1.2rem;
            object-fit: cover;
            object-position: top;
        }
        .title{
            font-family: Arial, Helvetica, sans-serif;
        }
    }
</style>