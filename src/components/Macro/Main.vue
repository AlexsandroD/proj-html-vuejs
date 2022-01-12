<template>
  <main>
    <Section1/>
    <Section2/>
    <Section3/>
    <Section4/>
    <Section5/>
    <Section6/>
  </main>
</template>

<script>
import Section1 from "../sections/Section1.vue";
import Section2 from "../sections/Section2.vue";
import Section3 from "../sections/Section3.vue";
import Section4 from "../sections/Section4.vue";
import Section5 from "../sections/Section5.vue";
import Section6 from "../sections/Section6.vue";


export default {
    name:"Main",
    components:{
      Section1,
      Section2,
      Section3,
      Section4,
      Section5,
      Section6,
    }
}
</script>

<style lang="scss" scoped>

</style>