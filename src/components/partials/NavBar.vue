<template>
  <nav class="navigation-bar">
      <Logo/>
      <div class="right-nav">
        <Menu/>
        <i class="far fa-user user"></i>
        <Button/>
      </div>
  </nav>
</template>

<script>
import Logo from "../micro/Logo.vue";
import Menu from "../micro/Menu.vue";
import Button from "../micro/Button.vue";
export default {
    name:"NavBar",
    components:{
        Logo,
        Menu,
        Button,
    },
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/global.scss";
        nav.navigation-bar{
        position: relative;
        z-index: 10;
        display: flex;
        align-items: center;
        justify-content: space-between;
        width: 60%;
        margin: auto;
        height: 80px;
        & .right-nav{
            font-size: 0.90rem;
            display: flex;
            align-items: center;
            & .user{
                color:#fff;
                margin: 0 10px;            }
        }
  }

 
</style>