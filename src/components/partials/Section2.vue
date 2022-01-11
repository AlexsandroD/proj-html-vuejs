<template>
    <div class="section2">
        <div class="container">
            <h5>road transport</h5>
            <h2>Main <span>Services</span></h2>
            <div class="container-text-button">
                <p>With all of this expertise and capability comes un unrivalled commitment to customer service. We will work hard to understand needs in order to develop a productive,long-term partnership.</p> 
                <a class="myButton">see all</a>
            </div>
            <div class="card-container">
                <Card v-for="(card,index) in cards" :key="index" :card="card"/>
            </div>
        </div>
    </div>
</template>

<script>
import Card from "../micro/Card.vue";
export default {
    name:"Section2",
    components:{
        Card,
    },
    data(){
        return{
            cards:[
                {
                    icon:"fas fa-memory",
                    name:"Technology",
                    description:"We are continually focused on developing technology solutions adapted to our client's needs."
                },
                {
                    icon:"fas fa-temperature-low",
                    name:"Reefer Cargo",
                    description:"Regular and frequent monitoring from the receipt of the loaded container to final destination."
                },
                {
                    icon:"fas fa-boxes",
                    name:"Dry Cargo",
                    description:"We work with most types of dry cargo, from valuable cargo to the most dangerous requi care."
                },

            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/global.scss";

    .section2{
        background-color: $shark;
        display:grid;
        & .container{
            padding: 90px 0px;
            width: 60%;
            margin: auto;
            & h5{
                color: $fountain-blue;
                text-transform: uppercase;
            }
            & h2{
                font-size: 2rem;
                font-weight: 700;
                color: #fff;
                margin: 15px 0;
                & span{
                    background-color:$blue-lagoon ;
                    padding: 0 10px;
                }
            }
            & .container-text-button{
                display: flex;
                justify-content: space-between;
                color: rgba(255, 255, 255, 0.522);
                
                p{
                    width: 80%;
                    font-size:.95rem;
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