<template>
     <div class="info-bar">
          <div class="item-container">
            <div class="items1">
                <div class="item">
                    <i class="fas fa-clock icon "></i>
                    <span>Open Hours: Mon - Sat - 9:00 - 18:00</span>
                </div>
            </div>

            <div class="items2">
                <div class="item phone">
                    <i class="fas fa-phone-alt"></i>
                    <span>+1(305) 1234-5678 </span>
                </div>
                <div class="item mail">
                    <i class="fas fa-envelope"></i>
                    <span>hello@example.com </span>
                </div>
                <div class="item icons">
                    <i class="fab fa-facebook-f icon"></i>
                    <i class="fab fa-twitter icon"></i>
                    <i class="fab fa-twitter icon"></i>                    
                </div>
            </div>
          </div>
      </div>
</template>

<script>
export default {
    name:"InfoBar"
}
</script>

<style lang="scss" scoped>

    @import "../../assets/style/global.scss";
.info-bar {
    position: relative;
    z-index: 10;
    width: 100%;
    height: 40px;
    background-color:$dark-blue;
.item-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    font-size: 0.70rem;
    color: #fff;
    height: 40px;
    width:60%;
    margin: auto;
    .items1{
        width: 50%;
        & .icon{
            margin-right: 5px;
        }
    }

    .items2 {
        display: flex;
        justify-content: flex-end;
        width: 50%;
        .item{
            margin: 0 10px;
            & .icon{
                margin: 0 15px
            }

            & span{
                margin-left: 5px;
            }
        }
    }
}

}

</style>