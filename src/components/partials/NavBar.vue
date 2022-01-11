<template>
  <nav class="navigation-bar">
      <div class="logo">
          <span class="left">nex</span>
          <span class="right">gen</span>
      </div>
      <div class="menu"></div>
      <div class="button"></div>
  </nav>
</template>

<script>
export default {
    name:"NavBar"
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/global.scss";
    nav.navigation-bar{
        position: relative;
        z-index: 10;
        display: flex;
        align-items: center;
        width: 70%;
        margin: auto;
        height: 80px;
        & .logo{
            text-transform: uppercase;
            font-weight: 700;
            letter-spacing:2px;
            color: white;
            & .left{
                border-radius: 15px 0px 0px 15px;
                padding-left: 15px;
                padding-top: 5px;
                padding-bottom: 5px;
                height: 80px;
                background-color:#0384844a;
                color:$blue-lagoon;
            }
        }
    }
 
</style>