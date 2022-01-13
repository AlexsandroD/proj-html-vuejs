<template>
    <div class="card">
        <div class="icons">
            <img :src="card.src" alt="">
        </div>
        <p>{{card.description}}</p>
        <div class="apici"><i class="fas fa-quote-right"></i></div>
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
    position: relative;
    padding: 35px;
    background-color: rgba(255, 255, 255, 0.07);
    border-radius: 10px;
    aspect-ratio: 1.2;
    transition:transform 0.3s;
    &:hover{
        transform: translateY(-8px);
    }
    & .icons{
    display:flex;
    filter: invert(1);
    img{
        width: 35%;
        margin-bottom: 15px;
        object-fit: cover;
    }
    & .icon-right a{
    color:$fountain-blue;
    }
    }
    & p{
        text-align: left;
        color: rgba(255, 255, 255, 0.522);
        font-size: 0.85rem;
       
    }
    .apici{
        position: absolute;
        bottom: 20px;
        right: 15px;
        font-size: 1.1rem;
        color: $mid-gray;
    }
}

</style>