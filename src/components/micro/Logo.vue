<template>
    <div class="logo">
          <span class="left">nex</span>
          <span class="right">gen</span>
      </div>
</template>

<script>
export default {
    name:"Logo"
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/global.scss";

     .logo{
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
                color:$fountain-blue;
            }
        }
    
</style>