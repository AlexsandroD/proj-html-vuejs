<template>
    <div class="section2">
        <div class="container">
            <h4>road transport</h4>
            <h2>Main Services</h2>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ab eum autem laboriosam modi distinctio facere ipsam officia doloribus! Expedita aut voluptatum asperiores unde provident quod atque eos reiciendis. Velit, eligendi.</p> 
            <a class="myButton">see all</a>
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
        height:600px;
        background-color: $shark;
        display:grid;
        & .container{
            background-color: green;
            width: 60%;
            margin: auto;
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