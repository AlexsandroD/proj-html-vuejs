<template>
        <div class="myButton opacity-"><a class="" href="#">view map</a></div>
</template>

<script>
export default {
    name:"ButtonForm2",
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/global.scss";
.myButton{
    border: 1px solid $blue-text;
    transition:0.3s ;
    &:hover{
         
                        opacity:1;
                        outline: $blue-lagoon solid 1px;
                        outline-offset: 5px;
                    
    }
    & a{
        color:$blue-text;
        text-transform:uppercase;
     
    }
}

</style>