<template>
        <div class="myButton opacity-"><a class="" href="#">Send</a></div>
</template>

<script>
export default {
    name:"ButtonForm",
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/global.scss";
.myButton{
    background-color: $blue-text;
    &:hover{
        opacity: 1;
    }
    & a{
        color:#fff;
        text-transform:uppercase;
     
    }
}

</style>