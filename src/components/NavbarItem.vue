<script>
export default {
    name: 'NavbarItem',
    data() {
        return {
            NavbarLinks: [
                {
                    text: 'HOME',
                },
                {
                    text: 'LANDING',
                },
                {
                    text: 'PAGES',
                },
                {
                    text: 'DOCS',
                },
                
            ],
        }
    },
}
</script>

<template>
    <div class="Navbar">
        <div class="img-container">
            <img src="../../public/img/logo-dark.png" alt="">
        </div>
        
        <div class="Links" v-for="NavbarLinks in NavbarLinks">
            <div><strong>{{ NavbarLinks.text }} </strong><i class="fa-solid fa-chevron-down"></i></div>
        </div>

        <div class="Icons-container">
            <i class="fa-solid fa-magnifying-glass glass"></i>
            <i class="fa-brands fa-github Small-icons"></i>
            <i class="fa-solid fa-dolly Small-icons"></i>
            <i class="fa-regular fa-user Small-icons"></i>
        </div>

    </div>
</template>

<style scoped>
    .Navbar{
        display: flex;
        justify-content: space-evenly;
        padding: 25px;
        background-color: #f8f9fc;
    }

    .Navbar img{
        width: 160px;
    }

    .Links:hover{
        color: #2f55d4;
        cursor: pointer;

    }

    .Icons-container{
        display: flex;
        gap: 10px;
        cursor: pointer;
    }

    .Small-icons{
        background-color: #eaeefb;
        color: #2f55d4;
        padding: 10px;
        border-radius: 5px;
        box-shadow: 5px 4px 10px gray;
    }

    .glass{
        padding: 10px;
        color: gray;
    }


</style>