<template>
    <li>
        <img v-scrollanimation src="../../assets/img/truck-1.png" alt="truck">
        <div class="text">
            <div>{{vehicle.type}}</div>
            <span>{{vehicle.maxKg}}</span>
        </div>
    </li>
</template>

<script>
export default {
    name:"Vehicles",
    props:{
        vehicle:{},
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/global.scss";
li{
    display: flex;
    align-items: center;
    &:nth-child(2){
    border-top:1px solid $silver-sand  ;
    border-bottom:1px solid $silver-sand ;
    }
    & img{
        background-color: #DAECED;
        padding:5px;
        width: 80px;
        margin: 10px 0;
            
          
        }
    & .text{
        margin: 0 15px;
        & div{
            font-weight: 600;
        }
        & span {
            color: $silver-sand;
            font-size: 0.8rem;
        }
    }
}

.before-enter{
    opacity: 0;
    transform: translateX(100%);
    transition: all  0.5s ease-in-out;
}

.enter{
    opacity: 1;
    transform: translateX(0);
}


</style>