<template>
    <div class="card">
        <div class="icons">
            <div class="icon-left"><i :class="card.icon"></i></div>
            <div class="icon-right"><i class="fas fa-arrow-right"></i></div>
        </div>
        <div class="h4">{{card.name}}</div>
        <p>{{card.description}}</p>
    </div>
</template>

<script>
export default {
    name:"Card",
    props: {
        card:{},
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/global.scss";
 .card{
    padding: 40px;
    background-color: #fff;
    border-radius: 10px;
    & .icons{
    display:flex;
    justify-content: space-between;
    & .icon-left{
    border-radius: 50%;
    font-size: 1.5rem;
    padding:10px;
    background-color: $blue-lagoon;
    color: $fountain-blue;
    }
    & .icon-right{
    color:$fountain-blue;
    }
    }
}

</style>