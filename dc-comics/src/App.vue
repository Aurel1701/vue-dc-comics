<template>
  <div id="app">
    <SiteHeader />
    <Goes />
    <SectionShop />
    <MainSection />
    <FooterSection />
    
  </div>
</template>

<script>
import SiteHeader from "@/components/HeaderComponents.vue";
import Goes from "@/components/HeaderContent.vue";
import SectionShop from "@/components/ContentShop.vue";
import MainSection from "@/components/MainList.vue";
import FooterSection from "@/components/FooterList.vue";
export default {
  name: 'App',
  components: {
    SiteHeader,
    Goes,
    SectionShop,
    MainSection,
    FooterSection,
  }
}
</script>

<style>
#app {
 
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  
  
}
</style>
