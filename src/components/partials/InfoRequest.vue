<template>
  <div class="info-container" >
      <div class="info" id="slide">
        <h5>logistics services</h5>
        <h1 id="slide2">cargo transport</h1>
        <p>Fractional or exclusive road cargo transportation to all regions,with small, medium and large vehicles</p>
        <ButtonInfo/>
        <BtnSecondary/>
      </div>
  </div>
</template>

<script>
import ButtonInfo from "../micro/ButtonInfo.vue";
import BtnSecondary from "../micro/BtnSecondary.vue";

export default {
    name:"InfoRequest",
    components:{
        ButtonInfo,
        BtnSecondary,
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/global.scss";

    .info-container{
        width: 60%;
        margin: 200px auto;
        position: relative;
        & .info{
            width:50%;
            & h5{
                font-size:0.90rem;
                color: $fountain-blue;
                text-transform: uppercase;
            }
            & h1{
                color:#fff;
                font-size: 4rem;
                text-transform: uppercase;
                font-weight: 900;

            }

            & p{
                color:rgba(255, 255, 255, 0.618);
                margin-bottom: 35px;
            }
        }
    }
    #slide {
    position: absolute;
    left: -800px;
    -webkit-animation: slide 0.5s forwards;
    -webkit-animation-delay: 2s;
    animation: slide 1s forwards;
    animation-delay: 1s;
}

@-webkit-keyframes slide {
    80%{ left: 100px;};

    100% { left: 0; }
}

@keyframes slide {
    80%{ left: 100px;};
    100% { left: 0; }
}

</style>