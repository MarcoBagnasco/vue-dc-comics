<template>
    <main>
        <!-- CONTENT SECT. -->
        <section class="content">
            <div class="container flex ai-center">
                <h2>--> Content goes here &lt;--</h2>
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
export default {
    name: 'Main',
    data() {
        return {
            tools: [
                {   
                    image: require('../assets/img/buy-comics-digital-comics.png'),
                    text: 'digital comics',
                },
                {   
                    image: require('../assets/img/buy-comics-merchandise.png'),
                    text: 'dc merchandise',
                },
                {   
                    image: require('../assets/img/buy-comics-subscriptions.png'),
                    text: 'subscription',
                },
                {   
                    image: require('../assets/img/buy-comics-shop-locator.png'),
                    text: 'comic shop locator',
                },
                {   
                    image: require('../assets/img/buy-dc-power-visa.svg'),
                    text: 'dc power visa',
                },
            ],
        }
    }
}
</script>

<style scoped>
    .container{
        height: 100%;
    }
    h2{
        font-size: 1.9em;
    }
    
    /* CONTENT SECT. */
    .content{
        height: 130px;
        background-color: #000;
    }

    /* TOOLS SECT. */
    .tools{
        height: 155px;
        background-color: #0282f9;
    }
    li{
        list-style: none;
        margin: 0 35px;
        text-transform: uppercase;
    }
    li:last-child{
        margin-right: 0;
    }
    li a{
        font-family: Arial, Helvetica, sans-serif;
        color: #fff;
    }
    li img{
        height: 55px;
        margin-right: 12px;
        vertical-align: middle;
    }
    li:last-child img{
        width: 55px;
    }
</style>