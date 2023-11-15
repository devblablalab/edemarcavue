<template>
   <div>
    <p>1</p>
    <p class="bold">R$7.700</p>
    <P>MiuMiu</P>
   </div>
</template>

<script>
export default {
  name: 'BrandItem'
 
}
</script>

<style scoped>

div {
    display: flex;
    gap: 1em;
    border-bottom: 2px dashed #7c7c7c;
    font-size: 1.3em;
}
.bold {
    font-weight: bold;
}

</style>