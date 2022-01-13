<template>
<a href="#">
    <div class="logo">
          <span class="left">nex</span>
          <span class="right"> gen</span>
    </div>
</a>
</template>

<script>
export default {
    name:"Logo"
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/global.scss";

    a{
        cursor: poiter;
    }
    .logo{  font-size: 1.5rem;
            text-transform: uppercase;
            font-weight: 700;
            letter-spacing:2px;
            color: white;
            & .left{
                border-radius: 20px 0px 0px 20px;
                padding-left: 15px;
                padding-top: 5px;
                padding-bottom: 5px;
                height: 80px;
                background-color:#0384844a;
                color:$fountain-blue;
            }
    }
    
</style>