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
    &:hover{
         opacity: 1;
    }
    & a{
        color:#fff;
        text-transform:uppercase;
        font-weight: 700;
    }
}

</style>