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
    border-radius: 15px;
    background-color: none;
    background-color: rgba(255, 255, 255, 0.104);
    transition:background-color 0.3s;
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