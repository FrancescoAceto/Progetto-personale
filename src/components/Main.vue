<script>
import CardsItem from './CardsItem.vue';
import PriceCardItem from './PriceCardItem.vue';

export default {
    name: "Main",
    data() {
        return {
            Cards: [
                'Modular',
                'Responsive',
                'Customizable',
                'Scalable',
            ],
            PriceCardItems: [
                'Basic',
                'Business',
                'Enterprise',
            ]
        }
    },
    components: { 
        CardsItem,
        PriceCardItem,
     },
}

</script>

<template>
    <div class="main-container">
        <div class="title-container">
            <h2>Key Features</h2>
            <h3>Start working with <span>Landrick</span> that can provide everything you need to generate awareness, drive traffic, connect.</h3>
        </div>
        <div class="Cards">
            <CardsItem v-for="card in Cards" :text="card"></CardsItem>
        </div>
        <div class="Quickstart">
            <h4>Quickstart</h4>
            <h1>Awesome isn't it? Let's dive in!</h1>
            <h3>Start working with <span>Landrick</span> that can provide everything you need to generate awareness, drive traffic, connect.</h3>
        </div>
        <div class="npm-box">
            <div class="column">
                <div class="white npm2">npm</div>
                <div class="white">nuget</div>
                <div class="white">spm</div>
                <div class="white">github</div>
            </div>
            <div class="npm-install">
                <div><span>$</span> npm install</div>
                <div><span>-g</span> claps.js</div>
            </div>
            <div class="Organize">
                <div><span><i class="fa-regular fa-circle-check"></i></span> Organize your data</div>
                <div><span><i class="fa-regular fa-circle-check"></i></span> Work with any team</div>
            </div>
        </div>
    </div>
    <div class="Tools-container">
                <div class="Tools">
                    <h2>Build tools and extensive documentation</h2>
                    <h3>You can combine all the Landrick templates into a single one, you can take a component from the Application theme and use it in the Website</h3>
                    <div><span><i class="fa-regular fa-circle-check"></i></span> Digital Marketing Solutions for Tomorrow</div>
                    <div><span><i class="fa-regular fa-circle-check"></i></span> Our Talented & Experienced Marketing Agency</div>
                    <div><span><i class="fa-regular fa-circle-check"></i></span> Create your own skin to match your brand</div>
                    <button><strong> Read More ></strong></button>
                </div>
                <div class="Tools-img">
                    <img src="../../public/img/1.png" alt="">
                </div>
            </div>
            <div class="Rates">
                <h1>Our rates for developer from landrick team</h1>
                <h3>Start working with <span>Landrick</span> that can provide everything you need to generate awareness, drive traffic, connect.</h3>
            </div>
            <div class="PriceCards">
                <PriceCardItem v-for="PriceCard in PriceCardItems" :type="PriceCard" :price="9.00" :description="'All the basics for business that are just getting started.'"></PriceCardItem>
            </div>
            <div class="Email-Us">
                <h1>Our rates for developer from landrick team</h1>
                <h3>Start working with <span>Landrick</span> that can provide everything you need to generate awareness, drive traffic, connect.</h3>
                <div>
                    <input type="text" placeholder="Email Address">
                    <button>Get Started</button>
                </div>
            </div>
            
</template>

<style scoped>
    .main-container{
        margin: 300px;
        margin-top: -20px;
    }
    .title-container{
        display: flex;
        flex-direction: column;
        padding: 70px;
    }

    .title-container h3{
        color: #adb5bd;
        width: 60%;
        margin-top: 20px;
    }

    .title-container span{
        color: #2f55d4;
    }

    .Cards{
        display: flex;
        justify-content: center;
        gap: 20px;
    }

    .Quickstart{
        display: flex;
        flex-direction: column;
        align-items: center;
        gap: 30px;
        padding: 200px;
    }

    .Quickstart h4{
        color: #2f55d4;
    }

    .Quickstart h3{
        color: #adb5bd;
        text-align: center;
    }

    .Quickstart span{
        color: #2f55d4;
    }

    .npm-box{
        width: 800px;
        background-color: #3c4858;
        height: 130px;
        margin: auto;
        padding-top: 20px;
        border-radius: 7px;
        padding: 20px;
    }

    .column{
        display: flex;
        justify-content: center;
        gap: 100px;
        border: 1px solid #adb5bd;
        border-radius: 10px;
        background-color: #4f5a69;
        padding: 10px;
    }

    .white{
        color: white;
    }

    .npm-install{
        display: flex;
        gap: 20px;
        padding-left: 20px;
        padding-top: 20px;
        color: #adb5bd;
    }

    .npm-install span{
        color: #2eca8b;
    }

    .npm2{
        background-color: #3c4858;
    }

    .Organize{
        display: flex;
        gap: 50px;
        margin-top: 50px;
        color: #adb5bd;
    }

    .Organize span{
        color: #2eca8b;
    }

    .Tools-container{
        display: flex;
        padding: 200px;
        gap: 200px;
    }

    .Tools{
        display: flex;
        flex-direction: column;
        width: 50%;
        gap: 10px;
    }

    .Tools-img img{
        width: 450px;
    }

    .Tools h3{
        color: #adb5bd;
        padding-bottom: 20px;
    }

    .Tools div{
        color: #adb5bd;
    }

    .Tools h2 {
        color: black;
        width: 50%;
        padding-bottom: 10px;
    }

    .Tools span{
        color: #2eca8b;
    }

    .Tools button{
        background-color: #2f55d4;
        width: 130px;
        height: 50px;
        padding: 10px;
        border-radius: 7px;
        color: white;
        border: none;
        margin-top: 20px;
    }

    .Rates{
        display: flex;
        flex-direction: column;
        gap: 30px;
        align-items: center;
        text-align: center;
    }

    .Rates h3{
        color: #adb5bd;
    }

    .Rates span{
        color: #2f55d4;
    }

    .PriceCards{
        display: flex;
        justify-content: center;
        gap: 20px;

        padding: 100px;
    }

    .Email-Us{
        display: flex;
        flex-direction: column;
        gap: 30px;
        align-items: center;
        text-align: center;
        padding-bottom: 100px;
    }

    .Email-Us h3{
        color: #adb5bd;
        width: 30%;
    }

    .Email-Us span{
        color: #2f55d4;
    }

    .Email-Us input{
        border-radius: 20px;
        border: 1px solid lightgray;
        padding: 13px;
        width: 400px;
    }

    .Email-Us button{
        border-radius: 20px;
        color: white;
        background-color: #2f55d4;
        border: none;
        padding: 13px;
        font-weight: bold;
        margin-left: -90px;
    }
</style>
