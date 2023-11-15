<template>
  <HeaderBrand></HeaderBrand>
  <div class="col">
     <ProjectBrand></ProjectBrand>
  <ShirtGif></ShirtGif>
    
  </div>
 <BrandItem></BrandItem>
</template>

<script>
import HeaderBrand from './components/HeaderBrand.vue';
import ProjectBrand from './components/ProjectBrand.vue';
import ShirtGif from './components/ShirtGif.vue';
import BrandItem from './components/BrandItem.vue';




export default {
    name: "App",
    components: { HeaderBrand, ProjectBrand, ShirtGif, BrandItem }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #7C7C7C;
  margin-top: 60px;
}

.col {
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>
