<template>
        <div class="myButton opacity-"><a class="" href="#">read more</a></div>
</template>

<script>
export default {
    name:"BtnSecondary",
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/global.scss";
.myButton{
    margin-left:  20px;
    border: 1px solid $fountain-blue;
    opacity: 0.5;
    transition: 0.3s;
    &:hover{
        opacity:1;
        outline: $blue-lagoon solid 1px;
        outline-offset: 5px;
    
    }
    & a{
        color:#fff;
        text-transform:uppercase;
        font-weight: 700;
    }
}

</style>