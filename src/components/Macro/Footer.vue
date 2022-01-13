<template>
 <footer>
     <div class="footer-top">
        <div class="container-card">
            <div class="cards">
                <div class="card">
                    <Logo/>
                    <p>A functional HTML Template for Corporate & Business.</p>
                    <div class="info">
                        <div class="icons"><i class="fas fa-phone-alt icon"></i><span>+1 (305) 1234-5678</span></div>
                        <div class="icons"><i class="fas fa-envelope icon"></i><span>hello@ecample.com</span></div>
                        <div class="icons"><i class="fas fa-map-marker-alt icon"></i><span>Main Avenue, 987</span></div>
                    </div>
                    <ButtonFooter/>
                </div>
                <div class="card-link">
                    <h2>About</h2>
                    <ul>
                        <li v-for="(about, index) in abouts" :key="index"><i class="fas fa-chevron-right arrow"></i><a href="">{{about}}</a></li>
                    </ul>
                </div>
                       <div class="card-link">
                    <h2>Transport</h2>
                    <ul>
                         <li v-for="(transport, index) in transports" :key="index"><i class="fas fa-chevron-right arrow"></i><a href="">{{transport}}</a></li>
                    </ul>
                </div>
                       <div class="card-link">
                    <h2>Support</h2>
                    <ul>
                         <li v-for="(support, index) in supports" :key="index"><i class="fas fa-chevron-right arrow"></i><a href="">{{support}}</a></li>
                    </ul>
                </div>
            </div>
         </div>
     </div>
     <div class="footer-bottom">
         <div class="text-container">
             <div class="left">Enjoy the low price. We are tracking any intention of piracy</div>
         <div class="right">
             <span>&copy;2020 nexgen </span>
             <span>is Proudly Powered by </span>
             <span>Codings.</span>
         </div>
         </div>
     </div>
 </footer>
</template>

<script>
import Logo from "../micro/Logo.vue";
import ButtonFooter from "../micro/ButtonFooter.vue";
export default {
    name:"Footer",
    components:{
        Logo,
        ButtonFooter,
    },
    data(){
        return{
        abouts:["The Company","Institutional","Social & Events","Innovations","Environment","Technology"],

        transports:["Industrialized","Chemicals","Packaged Liquids","Construction","Laminated wood","And others"],

        supports:["Responsability","Terms of Use","About Cookies","Privacy Policy","Accessibility","information"]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/global.scss";
footer{
    margin-top: 70px;
}
    .footer-top{
        display: grid;
        align-items: center;
        height: 500px;
        background-color: #111117;
    
        .cards{
            display: grid;
            grid-template-columns:repeat(auto-fill, calc(25% - 12px));
            column-gap: 15px;
            width: 60%;
            margin: auto;
            color: #fff;
            .card{
                p{
                    color:$text-gray;
                }
            }
            p{
                margin: 20px 0;
            }
            .info{
                color: $text-gray;
                .icons{
                    margin: 10px 0;
                    span{
                        margin: 0 10px;
                    }
                }
            }
            .card-link{
                padding: 35px;
                border-radius: 5px;
                background-color:rgba(128, 128, 128, 0.131);
                li{
                    margin: 10px 0;
                    a{
                        margin:0 10px;
                        color: $text-gray;
                        font-size: 0.8rem;
                    }
                }
            }
        }
    }

    .footer-bottom{
        display: grid;
        height:60px;
        background-color:black;
        .text-container{
            width: 60%;
            margin: auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            color:$text-gray;
            & span:nth-child(1){
                text-transform: uppercase;
            }
            & span:nth-last-child(1){
                color:$blue-lagoon;
            }
        }
    }
</style>