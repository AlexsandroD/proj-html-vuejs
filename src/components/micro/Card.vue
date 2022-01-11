<template>
    <div class="card">
        <div class="icons">
            <div class="icon-left"><i :class="card.icon"></i></div>
            <div class="icon-right"><a href="#"><i class="fas fa-arrow-right"></i></a></div>
        </div>
        <h4>{{card.name}}</h4>
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
    padding: 35px;
    background-color: rgba(255, 255, 255, 0.07);
    border-radius: 10px;
    aspect-ratio: 1.2;
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
    & .icon-right a{
    color:$fountain-blue;
    }
    }
    & h4{
        color:#fff;
        margin: 15px 0px;
    }
    & p{
        color: rgba(255, 255, 255, 0.522);
        font-size: 0.85rem;
    }
}

</style>