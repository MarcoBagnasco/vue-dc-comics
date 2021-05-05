<template>
    <header>
        <div class="container flex jc-between">
            <img src="../assets/img/dc-logo.png" alt="" class="logo">
            <nav>
                <ul class="flex">
                    <li v-for="(item, index) in navLinks" :key="index"   class="flex ai-center" :class="{active: item.current}"><a href="/">{{item.text}}</a></li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
export default {
    name: 'Header',
    data(){
        return {
            navLinks:[
                {
                    text: 'characters',
                    url: '/characters',
                    current: false,
                },
                {
                    text: 'comics',
                    url: '/comics',
                    current: false,
                },
                {
                    text: 'movies',
                    url: '/movies',
                    current: false,
                },
                {
                    text: 'tv',
                    url: '/tv',
                    current: false,
                },
                {
                    text: 'games',
                    url: '/games',
                    current: false,
                },
                {
                    text: 'collectibles',
                    url: '/collectibles',
                    current: false,
                },
                {
                    text: 'videos',
                    url: '/videos',
                    current: false,
                },
                {
                    text: 'fans',
                    url: '/fans',
                    current: false,
                },
                {
                    text: 'news',
                    url: '/news',
                    current: false,
                },
                {
                    text: 'shop',
                    url: '/shop',
                    current: false,
                },
            ],
        }
    }
}
</script>

<style scoped>
    header{
        height: 120px;
        background-color: #fff;
    }
    .container{
        height: 100%;
    }
    img{
        align-self: center;
        height: 80px;
    }
    ul{
        height: 100%;
        list-style: none;
    }
    li{
        position: relative;
        margin: 0 15px;
        overflow-y: hidden; ;
    }
    li:after{
        content: '';
        position: absolute;
        bottom: -6px;
        left: 0;
        width: 100%;
        height: 6px;
        background-color: #0282f9;
        transition: bottom .4s .1s;
    }
    li:hover:after,
    li.active:after{
       bottom: 0;
    }
    li a{
        text-transform: uppercase;
        font-weight: 500;
        color: #000;
        transition: color .2s;
    }
    li a:hover,
    li.active a{
        color: #0282f9;
    }
</style>