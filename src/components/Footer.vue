<template>
    <footer>
        <!-- TOP FOOTER -->
        <div class="top-footer">
            <div class="container flex jc-between">
                <!-- Menu -->
                <div class="menu flex">
                    <div class="list-menu">
                        <h3>dc comics</h3>
                        <ul>
                            <li><a href="/">Characters</a></li>
                            <li><a href="/">Comics</a></li>
                            <li><a href="/">Movies</a></li>
                            <li><a href="/">TV</a></li>
                            <li><a href="/">Games</a></li>
                            <li><a href="/">Videos</a></li>
                            <li><a href="/">News</a></li>
                        </ul>
                        <h3>shop</h3>
                        <ul>
                            <li><a href="/">Shop DC</a></li>
                            <li><a href="/">Shop DC Collectibles</a></li>
                        </ul>
                    </div>
                    <div class="list-menu">
                        <h3>dc</h3>
                        <ul>
                            <li><a href="/">Terms Of Use</a></li>
                            <li><a href="/">Privacy Policy (New)</a></li>
                            <li><a href="/">Ad Choices</a></li>
                            <li><a href="/">Advertising</a></li>
                            <li><a href="/">Jobs</a></li>
                            <li><a href="/">Subscriptions</a></li>
                            <li><a href="/">Talent Workshops</a></li>
                            <li><a href="/">CPSC Certificates</a></li>
                            <li><a href="/">Ratings</a></li>
                            <li><a href="/">Shop Help</a></li>
                            <li><a href="/">Contact Us</a></li>
                        </ul>
                    </div>
                    <div class="list-menu">
                        <h3>sites</h3>
                        <ul>
                            <li><a href="/">DC</a></li>
                            <li><a href="/">MAD Magazine</a></li>
                            <li><a href="/">DC Kids</a></li>
                            <li><a href="/">DC Universe</a></li>
                            <li><a href="/">DC Power Visa</a></li>
                        </ul>
                    </div>
                </div>
                <!-- Logo -->
                <img src="../assets/img/dc-logo-bg.png" alt="logo">
            </div>
        </div>

        <!-- BOTTOM FOOTER -->
        <div class="bottom-footer">
            <div class="container flex jc-between ai-center">
                <!-- Sign Up -->
                <div class="btn">sign-up now!</div>
                <!-- Social -->
                <div class="social flex ai-center">
                    <span class="follow">follow us</span>
                    <a href="https://www.facebook.com/dccomics" target="_blank">
                        <img src="../assets/img/footer-facebook.png" alt="facebook">
                    </a>
                    <a href="https://twitter.com/dccomics" target="_blank">
                        <img src="../assets/img/footer-twitter.png" alt="twitter">
                    </a>
                    <a href="https://www.youtube.com/channel/UCiifkYAs_bq1pt_zbNAzYGg" target="_blank">
                        <img src="../assets/img/footer-youtube.png" alt="youtube">
                    </a>
                    <a href="https://www.pinterest.it/dccomics/" target="_blank">
                        <img src="../assets/img/footer-pinterest.png" alt="pinterest">
                    </a>
                    <a href="https://www.periscope.tv/DCComics/1ZkKzezXwZdxv" target="_blank">
                        <img src="../assets/img/footer-periscope.png" alt="periscope">
                    </a>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'Footer',
}
</script>

<style scoped>
    .container{
        height: 100%;
    }
    /* TOP FOOTER */
    .top-footer{
        padding-top: 40px;
        height: 370px;
        background-image: url('../assets/img/footer-bg.jpg');
        background-size: cover;
        overflow: hidden;
    }
    /* Menu */
    h3{
        margin-bottom: 15px;
        text-transform: uppercase;
        font-size: 1.4em;
    }
    ul{
        margin: 0 30px 20px 0;
        list-style: none;
    }
    li{
        margin-bottom: 3px;
    }
    li a{
        font-family: Arial, Helvetica, sans-serif;
        font-size: 0.85em;
        color: #858585;
    }
    /* Logo */
    .top-footer img{
        height: 560px;
        position: relative;
        bottom: 140px;
    }

    /* BOTTOM FOOTER */
    .bottom-footer{
        height: calc(100vh - 775px);
        background-color: #303030;
    }
    /* Sign Up */
    .btn{
        padding: 13px;
        text-transform: uppercase;
        font-family:Arial, Helvetica, sans-serif;
        font-weight: bold;
        font-size: 1.15em;
        border: 2px solid #0282f9;
        cursor: pointer;
    }
    /* Social */
    .follow{
        margin-right: 5px;
        text-transform: uppercase;
        font-weight: bold;
        font-size: 1.6em;
        color: #0282f9;
    }
    .bottom-footer img{
        margin-left: 20px;
    }
</style>