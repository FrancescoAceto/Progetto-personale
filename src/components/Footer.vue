<script>
export default {
    name: 'Footer',
}
</script>

<template>
    <div class="Footer-container">
        <div class="Startwork">
           <img src="../../public/img/logo-light.png" alt="">
           <p>Start Working with Ladnrick that can provide everything you need to generate awareness, drive traffic, connect</p>
           <div class="socials">
            <div><i class="fa-brands fa-facebook-f"></i></div>
            <div><i class="fa-brands fa-instagram"></i></div>
            <div><i class="fa-brands fa-twitter"></i></div>
            <div><i class="fa-brands fa-linkedin-in"></i></div>
           </div>
        </div>
        <div class="Company">
            <h3>Company</h3>
            <div><i class="fa-solid fa-chevron-right"></i> About Us</div>
            <div><i class="fa-solid fa-chevron-right"></i> Services</div>
            <div><i class="fa-solid fa-chevron-right"></i> Team</div>
            <div><i class="fa-solid fa-chevron-right"></i> Pricing</div>
            <div><i class="fa-solid fa-chevron-right"></i> Project</div>
            <div><i class="fa-solid fa-chevron-right"></i> Careers</div>
            <div><i class="fa-solid fa-chevron-right"></i> Blog</div>
            <div><i class="fa-solid fa-chevron-right"></i> Login</div>
        </div>
        <div class="Useful-links">
            <h3>Useful Links</h3>
            <div><i class="fa-solid fa-chevron-right"></i> Terms of Services</div>
            <div><i class="fa-solid fa-chevron-right"></i> Privacy Policy</div>
            <div><i class="fa-solid fa-chevron-right"></i> Documentation</div>
            <div><i class="fa-solid fa-chevron-right"></i> Changelog</div>
            <div><i class="fa-solid fa-chevron-right"></i> Components</div>
        </div>
        <div class="Newsletter">
            <h3>Newsletter</h3>
            <div>Sign up and receive the lastest tips via email </div>
            <div class="WriteEmail">
                <div>Write your email <strong>*</strong></div>
                <input type="text" placeholder="Your Email:">
                <button>Subscribe</button>
            </div>
        </div>
    </div>
    <hr>
    <div class="endbar">
        <div>
            <i class="fa-regular fa-copyright"></i>
            2020 Landrick. Design with <i class="fa-solid fa-heart"></i> by Francesco.
        </div>
        <div class="payment">
            <div><img src="../../public/img/american-ex.png" alt=""></div>
            <div><img src="../../public/img/discover.png" alt=""></div>
            <div><img src="../../public/img/master-card.png" alt=""></div>
            <div><img src="../../public/img/paypal.png" alt=""></div>
            <div><img src="../../public/img/visa.png" alt=""></div>
        </div>
    </div>
</template>

<style scoped>
    .Footer-container{
        display: flex;
        gap: 20px;
        justify-content: center;
        width: 100%;
        background-color: #202942;
        padding: 50px;
        color: white;
    }

    .Startwork{
        display: flex;
        flex-direction: column;
        width: 25%;
        gap: 20px;
    }

    .Startwork p{
        color: white;
        width: 30%;
    }

    .Startwork img{
        width: 160px;
    }

    .socials{
        display: flex;
        gap: 5px;
        color: white;
        cursor: pointer;
    }

    .socials div{
        border: 1px solid white;
        border-radius: 5px;
        padding: 7px;
        cursor: pointer;
    }

    .Company{
        width: 25%;
        display: flex;
        flex-direction: column;
        gap: 20px;
        cursor: pointer;
    }

    .Useful-links{
        width: 25%;
        display: flex;
        flex-direction: column;
        gap: 20px;
        cursor: pointer;
    }

    .Newsletter{
        display: flex;
        flex-direction: column;
        gap: 20px;
        padding-bottom: 20px;
    }

    .WriteEmail{
        display: flex;
        flex-direction: column;
        gap: 20px;
    }

    .WriteEmail strong{
        color: #e13f52;
    }

    .WriteEmail input{
        border: none;
        padding: 10px;
        border-radius: 5px;
        color: white;
        background-color: #27314f;
    }

    .WriteEmail button{
        border: none;
        padding: 10px;
        border-radius: 5px;
        color: #2c4cb5;
        background-color: #222e51;
    }

    .endbar{
        display: flex;
        justify-content: space-around;
        align-items: center;
        background-color: #202942;
        color: white;
        padding: 30px;
    }

    .payment{
        display: flex;
        gap: 5px;
    }

    .payment img{
        width: 40px;
    }
</style>
