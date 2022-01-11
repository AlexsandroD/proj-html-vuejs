<template>
  <div class="info-container">
      <div class="info">
        <h5>logistics services</h5>
        <h1>cargo transport</h1>
        <p>Fractional or exclusive road cargo transportation to all regions,with small, medium and large vehicles</p>
        <Button/>
        <BtnSecondary/>
      </div>
  </div>
</template>

<script>
import Button from "../micro/Button.vue";
import BtnSecondary from "../micro/BtnSecondary.vue";

export default {
    name:"InfoRequest",
    components:{
        Button,
        BtnSecondary,
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/global.scss";

    .info-container{
        width: 60%;
        margin: 80px auto;
        height: 300px;
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

            }

            & p{
                color:rgba(255, 255, 255, 0.618);
                margin-bottom: 35px;
            }
        }
    }
</style>