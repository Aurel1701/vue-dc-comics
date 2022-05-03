<template>
  <div id="app">
    <SiteHeader />
    <Goes />
    <SectionShop />
    
  </div>
</template>

<script>
import SiteHeader from "@/components/HeaderComponents.vue";
import Goes from "@/components/HeaderContent.vue";
import SectionShop from "@/components/ContentShop.vue";
export default {
  name: 'App',
  components: {
    SiteHeader,
    Goes,
    SectionShop,
  }
}
</script>

<style>
#app {
 
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  
  
}
</style>
