<template>
  <main>
    <Section1/>
    <Section2/>
    <Section3/>
  </main>
</template>

<script>
import Section1 from "../partials/Section1.vue";
import Section2 from "../partials/Section2.vue";
import Section3 from "../partials/Section3.vue";
export default {
    name:"Main",
    components:{
      Section1,
      Section2,
      Section3,

    }
}
</script>

<style lang="scss" scoped>

</style>