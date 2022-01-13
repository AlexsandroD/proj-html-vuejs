<template>
<div class="filter-container">
  <nav class="navigation-bar" :class="className">
      <Logo/>
      <div class="right-nav">
        <Menu/>
        <i class="far fa-user user"></i>
        <Button/>
      </div>
  <div class="filter">
  </div>
  </nav>
</div>
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
    data(){
      return{
        className:"",
      }
    },
    created(){
      window.addEventListener("scroll", () => {
        if(window.scrollY > 0){
          this.className = "scroll";
        }else{
          this.className = "";
        }
      } )
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/global.scss";
        nav.navigation-bar{
        position: fixed;
        top: 60px;
        left: 50%;
        transform: translateX(-50%);
        z-index: 999;
        display: flex;
        align-items: center;
        justify-content: space-between;
        width: 60%;
        margin: auto;
        transition: background-color 0.3s;
        border-radius: 20px 20px 20px 20px;
        &.scroll{
            background-color:rgba(0, 0, 0, 0.679);
        }
        & .right-nav{
            font-size: 0.90rem;
            display: flex;
            align-items: center;
            & .user{
                color:#fff;
                margin: 0 10px;
                transition: transform 0.5s;
                &:hover{
                  transform: rotate(360deg);
                  color:$fountain-blue;
                } 
           }
        }

  }
  .filter-container{
    position: relative;
    .filter{
      border-radius: 15px 4px 4px 15px;
      position: absolute;
      top: 0;
      right: 0px;
      left: 0;
      bottom: 0;
      z-index: -1;
    }
    

  }

 
</style>