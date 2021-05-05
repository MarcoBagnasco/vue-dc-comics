<template>
    <main>
        <!-- CONTENT SECT. -->
        <section class="content">
            <div class="hero">
                <img src="../assets/img/jumbotron.jpg" alt="hero">
            </div>
            <div class="series">
                <div class="container flex">
                    <Album
                        v-for="(album, index) in albums"
                        :key="index"
                        :album="album"
                    />
                    <div class="btn-load">load more</div>
                </div>
            </div>
        </section>

        <!-- TOOLS SECT. -->
        <section class="tools">
            <div class="container flex ai-center">
                <ul class="flex ai-center">
                    <li v-for="(item, index) in tools" :key="index"><a href="/"><img :src="item.image" :alt="item.text">{{item.text}}</a></li>
                </ul>
            </div>
        </section>
    </main>
</template>

<script>
import Album from '@/components/Album.vue';

// Data
import Comics from '@/data/dc-comics.js';
import Tools from '@/data/tools.js';

export default {
    name: 'Main',
    components: {
        Album,
    },
    data() {
        return {
            albums: Comics,
            tools: Tools,
        };
    }
}
</script>

<style scoped lang="scss">
    main{
        text-transform: uppercase;
    }
    .container{
        height: 100%;
        flex-wrap: wrap;
        justify-content: center;
    }
    /* CONTENT SECT. */
    .content{
        // Hero
        .hero{
            height: 400px;
            overflow: hidden;
        }

        // Series
        .series{
            position: relative;
            padding-top: 55px;
            padding-bottom: 20px;
            background-color: #1c1c1c;
            &::before{
                content: 'current series';
                position: absolute;
                bottom: 100%;
                left: 315px;
                transform: translateY(50%);
                padding: 9px 25px;
                color: #fff;
                font-size: 1.8rem;
                font-weight: bold;
                background-color: #0282f9;
            }
            .btn-load{
                padding: 9px 60px;
                font-weight: bold;
                background-color: #0282f9;
            }
        }
    }

    /* TOOLS SECT. */
    .tools{
        height: 155px;
        background-color: #0282f9;
    }
    li{
        list-style: none;
        margin: 0 35px;
        a{
            font-family: Arial, Helvetica, sans-serif;
            color: #fff;
        }
        img{
            height: 55px;
            margin-right: 12px;
            vertical-align: middle;
        }
        &:last-child{
            margin-right: 0;
            img{
                width: 55px;
            }
        }
    }
</style>