<template>
<div class="logo-section-1">
    <span class="logo-left"><i class="far fa-gem diamante"></i><span>Excellence</span> </span>
    <span class="logo-right">in Transport</span>
</div>
</template>

<script>
export default {
    name:"LogoSection1",
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/global.scss";
    .logo-section-1{
            font-weight: 700;
            color: white;
            margin: 20px 0;
            font-size:1.8rem;
            & .logo-left{
                color:$blue-lagoon ;
                background-color:#daeced;
                & span{
                    padding-right:5px;
                }
                border-radius:2px;
                padding: 5px;
                height: 80px;
                color:$fountain-blue;
                & .diamante{
                    margin: 0 5px;
                }
            }

            & .logo-right{
                color:black;
                margin: 0 5px;
            }
    }
</style>