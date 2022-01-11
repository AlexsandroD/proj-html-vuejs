<template>
    <div class="container">
        <div class="left">
            <h5>who we are</h5>
            <LogoSection1/>
            <div class="text-container">
                <p class="text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptates quisquam eaque dolor soluta rerum doloremque nesciunt. Sequi at obcaecati porro aspernatur aliquid suscipit accusamus ullam eos, quia cupiditate eum praesentium.</p>
                <p class="text">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Dolore, quae explicabo. Totam error, sed veritatis ipsa quibusdam distinctio ab consectetur molestiae eos hic placeat blanditiis vero dolorem quidem quisquam delectus.</p>
                <p class="text line">Lorem ipsum dolor sit amet consectetur adipisicing elit. Quam temporibus, eveniet autem repellat eaque cum nemo illum omnis porro maxime iure sunt odio, id voluptates sapiente culpa labore. Aliquid, rerum?</p>
                <p class="text">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Eos nesciunt nsequatur rem quasi voluptates!</p>
                <ul class="text">
                    <li>Lorem ipsum dolor sit amet</li>
                    <li>Consectetur adipisicing elit</li>
                    <li>Voluptates quisquam eaque dolor</li>
                    <li>Molestiae eos hic placeat</li>
                    <li>Amet consectetur adipisicing eli</li>           
                </ul>
            </div>
        </div>
        <div class="right">
            <h4>Vehicle Types</h4>
            <ul>
                <Vehicles v-for="(vehicle,index) in vehicles" :key="index" :vehicle="vehicle"/>
            </ul>
            <h4 class="certifications">Certifications</h4>
            <img src="../../assets/img/certificate.png" alt="certifications">
            <img src="../../assets/img/certificate.png" alt="certifications">
        </div>
    </div>
</template>

<script>
import LogoSection1 from "../micro/LogoSection1.vue";
import Vehicles from "../micro/Vehicles.vue";
export default {
    name:"Section1",
    components: {
        LogoSection1,
        Vehicles,
    },
    data(){
        return{
            vehicles:[
                {
                    type:"Light",
                    maxKg:"Max Weight 1200 kg"
                },
                {
                    type:"Medium",
                    maxKg:"Max Weight 6000 kg"
                },
                {
                    type:"Heavy",
                    maxKg:"Max Weight 24000 kg"
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/global.scss";
.container{
    display: flex;
    justify-content:space-between;
    padding:70px 0;
    width:60%;
    margin: auto;
    & .left{
        width: 65%;
        & h5{
            color:$fountain-blue;
            text-transform: uppercase;
        }
        .text-container{
            & .text{
                color:$silver-sand;
                font-size: 0.8rem;
                margin: 10px 0;
                &.line{
                    border-left: 1px solid black;
                    padding: 10px;
                }
            }
            li{
                margin-top: 5px;
                &:before{
                    content: "\2022";
                    margin-right:10px;
                }
            }
        }
    }
    & .right{
        width: 28%;
        & ul{
            margin-top: 25px;
        }
        h4.certifications{
            font-weight: 700;
            margin-top: 30px;
        }
        & img{
            margin: 10px 0;
            padding: 5px;
            width: 50%;
        }
    }

}

</style>