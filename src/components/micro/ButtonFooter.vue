<template>
        <div class="myButton opacity-"><a class="" href="#">get in touch</a></div>
</template>

<script>
export default {
    name:"ButtonFooter",
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/global.scss";
.myButton{
    margin-top: 30px;
    border: 1px solid $blue-text;
    &:hover{
        opacity: 1;
    }
    & a{
        color:#fff;
        text-transform:uppercase;
     
    }
}

</style>