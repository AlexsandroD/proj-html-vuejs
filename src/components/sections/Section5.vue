<template>
    <div class="section5">
        <div class="container">
            <h5>road transport</h5>
            <h2>Trusted <span>Feedback</span></h2>
                <p>We work intensively in search of ideals that can add up in the lives of our customers. This is what moves us and we are grateful for the recognition.</p> 
            <div class="card-container">
                <CardSec5 v-for="(card,index) in cards" :key="index" :card="card"/>
            </div>
        </div>
    </div>
</template>

<script>
import CardSec5 from "../micro/CardSec5.vue";
export default {
    name:"Section5",
    components:{
        CardSec5,
    },
    data(){
        return{
            cards:[
                {
                    src:require("../../assets/img/logo-1.png"),
                    description:"   Lorem ipsum dolor sit amet, consectetur adipisicing elit. Optio atque labore fuga a facilis error velit. Temporibus assumenda magnam beatae placeat illum, vitae deserunt, minus accusantium quidem itaque, ad obcaecati."
                },
                {
                    src:require("../../assets/img/logo-2.png"),
                    description:" Lorem ipsum dolor sit amet, consectetur adipisicing elit. Optio atque labore fuga a facilis error velit. Temporibus assumenda magnam beatae placeat illum, vitae deserunt, minus accusantium quidem itaque, ad obcaecati."
                },
                {
                    src:require("../../assets/img/logo-3.png"),
                    description:"   Lorem ipsum dolor sit amet, consectetur adipisicing elit. Optio atque labore fuga a facilis error velit. Temporibus assumenda magnam beatae placeat illum, vitae deserunt, minus accusantium quidem itaque, ad obcaecati."
                },

            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/global.scss";

    .section5{
        background-color: $shark;
        & .container{
            padding-top: 120px;
            padding-bottom: 60px;
            width: 60%;
            margin: auto;
            text-align: center;
            & h5{
                color: $fountain-blue;
                text-transform: uppercase;
            }
            & p{
                color: rgba(255, 255, 255, 0.522);
            }
            & h2{
                font-size: 2rem;
                font-weight: 700;
                color: #fff;
                margin: 15px 0;
                & span{
                    background-color:#0E272D ;
                    padding: 0 10px;
                }
                .myButton{
                    text-transform: uppercase;
                    color:#fff;
                    border: 1px solid $blue-lagoon;
                    padding: 5 10px;
                }
            }
            & .card-container{
            margin: 60px auto;
            display: grid;
            justify-content: center;
            grid-template-columns:repeat(auto-fill, 32%);
            column-gap:15px;
            row-gap: 20px;
            }
        }
    }
</style>