<script>
import { stringifyExpression } from '@vue/compiler-core';

export default {
    name: 'CardsItem',
    data() {
        return {
            
        }
    },
    props: {
        icon: String,
        text: String,
    }
}
</script>

<template>
    <div class="Mode-card">
        <div class="mini-icon"><i class="fa-solid fa-chalkboard-user"></i></div>
        <div><strong>{{ text }}</strong></div>
        <div class="card-sub">Composed in a pseudo-latin language wich more or less corresponds.</div>
        <div class="Read-more">Read More ></div>
    </div>
</template>

<style scoped>
    .Mode-card{
        display: flex;
        flex-direction: column;
        gap: 20px;
        width: 250px;
        height: 280px;

        border: 1px solid lightgray;
        border-radius: 10px;
        padding: 30px;
    }

    .mini-icon{
        font-size: 30px;
        color: #2f55d4;
        background-color: #eaeefb;
        padding: 20px;
        width: 80px;
        border-radius: 10px;
        cursor: pointer;
    }

    .card-sub{
        color: #adb5bd;
    }

    .Read-more{
        color: #2f55d4;
        cursor: pointer;
    }
</style>