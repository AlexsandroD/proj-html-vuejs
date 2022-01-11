<template>
  <header>
      <div class="filter"></div>
      <InfoBar/>
      <NavBar/>
      <InfoRequest/>
  </header>
</template>

<script>
import InfoBar from "../partials/InfoBar.vue";
import NavBar from "../partials/NavBar.vue";
import InfoRequest from "../partials/InfoRequest.vue";
export default {
    name:"Header",
    components:{
        InfoBar,
        NavBar,
        InfoRequest
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/global.scss";
header{
    position: relative;
    z-index: 1;
    height: 700px;
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
        z-index: -1;
   }
    
}


</style>