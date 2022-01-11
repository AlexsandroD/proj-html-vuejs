<template>
  <div class="menu">
      <ul>
          <li v-for="(voice, index) in menuVoices" :key="index"><a href="">{{voice}}</a></li>
      </ul>
  </div>
</template>

<script>
export default {
    name:"Menu",
    data(){
        return{
            menuVoices: ["home","about","services","process","testimonials"]
        }
    }

}
</script>

<style lang="scss" scoped>
@import "../../assets/style/global.scss";
 .menu{
     & ul{
         display: flex;
         & li{
             margin: 0 10px;
             & a{
                 text-transform: uppercase;
                 color: white;
             }
             &:hover a{
                 color: $fountain-blue;
             }
         }
     }
 }

 
</style>