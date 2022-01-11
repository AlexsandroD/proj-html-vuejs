<template>
        <div class="myButton opacity-"><a class="" href="#">get in touch</a></div>
</template>

<script>
export default {
    name:"Button",
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/global.scss";
.myButton{
    background-color: $fountain-blue;
    margin-left:  10px;
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