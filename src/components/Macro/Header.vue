<template>
  <header>
      <div class="filter"></div>
      <InfoBar/>
      <NavBar/>
  </header>
</template>

<script>
import InfoBar from "../partials/InfoBar.vue";
import NavBar from "../partials/NavBar.vue";
export default {
    name:"Header",
    components:{
        InfoBar,
        NavBar
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/global.scss";
header{
    position: relative;
    height: 600px;
    background-image: url("../../assets/img/bg-9.jpg");
    background-repeat: no-repeat;
    background-size:cover;
    & .filter{
        position:absolute;
        background-color: rgba(0, 0, 0, 0.398);
        top:0;
        right:0;
        bottom: 0;
        left: 0;
   }
    
}


</style>