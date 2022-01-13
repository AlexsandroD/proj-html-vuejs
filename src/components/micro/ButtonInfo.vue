<template>
        <div class="myButton"><a class="" href="#">get in touch</a></div>
</template>

<script>
export default {
    name:"Button",
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/global.scss";
.myButton{
    background-color:$fountain-blue;
    transition:opacity 0.5s;
    opacity: 0.7;
    &:hover{
        background-color:$fountain-blue;
        opacity: 1;
    }
    & a{
        color:#fff;
        text-transform:uppercase;
        font-weight: 700;
    }
    
}

</style>