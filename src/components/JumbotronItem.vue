<script>
export default {
    name: 'JumbotronItem'
}
</script>

<template>
    <div class="Jumbotron">
        <div class="Toolset">
            <div class="Development"><strong>Development</strong></div>
            <div class="Dev-Title"><h1>A Complete Developer Toolset</h1></div>
            <div class="Dev-Subtitle"><h3>Launch Your Career and benefit from our expertise on designing and managing conversion centered bootstrap4 html page.</h3></div>
            <div class="Buttons">
                <button class="Button1"><strong>Get Started</strong></button>
                <button class="Button2"><strong>Documentation</strong></button>
            </div>
            <div class="Dev-Subtitle"><h3>Current Version: v2.6.0</h3></div>
        </div>

        <div class="Jumbo-img">
            <img src="../../public/img/about.png" alt="">
        </div>
    </div>
    <hr>
    <div class="brands">
            <div><img src="../../public/img/amazon.svg" alt=""></div>
            <div><img src="../../public/img/google.svg" alt=""></div>
            <div><img src="../../public/img/lenovo.svg" alt=""></div>
            <div><img src="../../public/img/paypal.svg" alt=""></div>
            <div><img src="../../public/img/shopify.svg" alt=""></div>
            <div><img src="../../public/img/spotify.svg" alt=""></div>
        </div>    
</template>

<style scoped>
    .Jumbotron{
        background-color: #f8f9fc;
        display: flex;
        flex-direction: center;
        padding: 150px;
        margin: auto;
    }

    .Toolset{
        display: flex;
        flex-direction: column;
        gap: 20px;
    }

    .Development{
        color: #2f55d4;
        background-color: #eaeefb;
        border-radius: 10px;
        width: 110px;
        padding: 2px;
        border: 0.5px solid lightgray;
    }

    .Dev-Title{
        width: 300px;
    }

    .Dev-Subtitle{
       width: 60%;
       color: #adb5bd;
    }

    .Buttons{
        display: flex;
        gap: 10px;
    }

    .Button1 {
        padding: 10px;
        border-radius: 5px;
        border: none;
        background-color: #2f55d4;
        color: white;
        cursor: pointer;
    }

    .Button2{
        padding: 10px;
        border-radius: 5px;
        color: #2f55d4;
        border: 1px solid #2f55d4;
        cursor: pointer;
    }

    .brands{
        display: flex;
        justify-content: center;
        gap: 70px;
        padding: 70px;
        background-color:#f8f9fc;
    }
    .brands img{
        width: 80px;
    }

</style>