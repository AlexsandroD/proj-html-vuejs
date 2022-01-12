<template>
  <section class="section6">
        <div class="container">
        <div class="left">
            <h6>send a message</h6>
            <h2>Get in <span>Touch</span></h2>
            <p class="text">We will respond to you messages as soon as possible.</p>
            <Form/>
        </div>
        <div class="right">
            <h4>Example Inc.</h4>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
            <p>present diam lacus, dapitus sed imperdiet consectetur</p>

            <div class="info">
                <div class="icons"><i class="fas fa-phone-alt icon"></i><span>+1 (305) 1234-5678</span></div>
                <div class="icons"><i class="fas fa-envelope icon"></i><span>hello@ecample.com</span></div>
                <div class="icons"><i class="fas fa-map-marker-alt icon"></i><span>Main Avenue, 987</span></div>
            </div>
            <ButtonForm2/>
        </div>
    </div>
  </section>
</template>

<script>
import Form from "../partials/Form.vue";
import ButtonForm2 from "../micro/ButtonForm2.vue";
export default {
    name:"Section6",
    components:{
        Form,
        ButtonForm2,
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/global.scss";
.section6{
    height: 500px;
    .container{
    display: flex;
    justify-content:space-between;
    padding:70px 0;
    width:60%;
    margin: auto;
    & .left{
        width: 65%;
        & h6{
            font-size: 0.6rem;
            color:$blue-text;
            text-transform: uppercase;
            margin-bottom: 20px;
        }
        h2{
            font-weight: 900;
            margin: 10px 0;
            font-size: 1.8rem;
            span{
                padding: 3px 10px;
                background-color:$background-blue;
                color: $blue-text;
            }
        }
        p{
            margin: 25px 0;
        }
    }
    & .right{
        width: 30%;
        p{
            margin: 15px 0;
            font-size: 0.7rem;
            color: gray;
        }
        .info{
            margin: 20px 0;
            .icons{
                
                display:flex;
                align-items: center;
                & span{
                    color: $blue-text;
                    margin: 0px 5px;
                }
                margin: 10px 0;
                .icon{
                    width: 30px;
                    height: 30px;
                    border-radius: 50%;
                    background-color:$background-blue;
                    padding: 8px;
                    color:$blue-text;
                   
                }
            }           
        }
    }

}
}
</style>