<script>
export default {
    name: 'PriceCardItem',

    data() {
        return {
            
        }
    },
    props: {
        type: String,
        price: Number,
        description: String,
    }
}
</script>

<template>
    <div class="PriceCard">
        <div class="plan"><strong>{{ type }}</strong></div>
        <h1>${{ price }}.00</h1>
        <div>Per Month</div>
        <div>{{ description }}</div>
        <hr>
        <div><span><i class="fa-regular fa-circle-check"></i></span> Full Access</div>
        <div><span><i class="fa-regular fa-circle-check"></i></span> Enhanced Security</div>
        <div><span><i class="fa-regular fa-circle-check"></i></span> Source Files</div>
        <div><span><i class="fa-regular fa-circle-check"></i></span> 1 Domain Free</div>
        <div><span><i class="fa-regular fa-circle-check"></i></span> Enchanced Security</div>
        <div class="BuyNow"><button>Buy Now</button></div>
        <div>*No credit card required</div>
    </div>
</template>

<style scoped>
    .PriceCard{
        display: flex;
        flex-direction: column;
        gap: 20px;

        border: 1px solid lightgray;
        border-radius: 10px;
        padding: 30px;
        box-shadow: 1px 5px 5px gray;
    }

    .PriceCard div{
        color: #adb5bd;
    }

    .PriceCard strong{
        color: #2f55d4;
    }

    .PriceCard span{
        color: #2f55d4;
    }

    .PriceCard button{
        color: white;
        background-color: #2f55d4;
        border: none;
        padding: 15px;
        text-align: center;
        width: 100%;
        border-radius: 10px;
        font-weight: bold;
        font-size: 15px;
    }

    .BuyNow{
        display: flex;
        justify-content: center;
    }
   

    .plan{
        background-color: #eaeefb;
        padding: 15px;
        width: 30%;
        border-radius: 30px;
        border: 1px solid lightgray;
        text-align: center;
    }
</style>