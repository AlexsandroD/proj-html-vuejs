<template>
  <div class="card">
    <div class="icons">
      <div class="icon-left"><i :class="card.icon"></i></div>
      <div class="icon-right">
        <a href="#"><i class="fas fa-arrow-right"></i></a>
      </div>
    </div>
    <h4>{{ card.name }}</h4>
    <p>{{ card.description }}</p>
  </div>
</template>

<script>
export default {
  name: "Card",
  props: {
    card: {},
  },
};
</script>

<style lang="scss" scoped>
@import "../../assets/style/global.scss";
.card {
  padding: 35px;
  background-color: rgba(255, 255, 255, 0.07);
  border-radius: 10px;
  aspect-ratio: 1.2;
  transition:transform 0.3s;
    &:hover{
        transform: translateY(-8px);
    }
  & .icons {
    display: flex;
    justify-content: space-between;
    & .icon-left {
      display:grid;
      place-items: center;
      flex-shrink: 0;
      width: 50px;
      height: 50px;
      border-radius: 50%;
      font-size: 1.5rem;
      background-color: $blue-lagoon;
      color: $fountain-blue;
    }
    .icon-right{
         display:grid;
          place-items: center;
        width: 30px;
        height: 30px;
        color: $fountain-blue;
        transition: 0.3s ease-in-out;
      & a{
          color:$fountain-blue;
      }
      &:hover{
          position: relative;
          width: 30px;
          height: 30px;
          color:$smalt-blue;
          border-radius:50%;
          background-color: $blue-lagoon
      }
    }
    
  }
  & h4 {
    color: #fff;
    margin: 15px 0px;
  }
  & p {
    color: rgba(255, 255, 255, 0.522);
    font-size: 0.85rem;
  }
}
</style>
