<template>
  <nav class="navigation-bar">
      <Logo/>
      <div class="right-nav">
        <Menu :menu="menuVoices"/>
        <i class="far fa-user user"></i>
        <div class="myButton"><a class="" href="#">get in touch</a></div>
      </div>
  </nav>
</template>

<script>
import Logo from "../micro/Logo.vue";
import Menu from "../micro/Menu.vue";
export default {
    name:"NavBar",
    components:{
        Logo,
        Menu,
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
            & .myButton{
                background-color: $fountain-blue;
                margin-left:  10px;
                & a{
                    color:#fff;
                    text-transform:uppercase;
                    font-weight: 700;
                }
            }
        }
  }

 
</style>