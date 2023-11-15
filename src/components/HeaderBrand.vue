<template>
    <header>
        <p>por <br> BlaBlaLab</p>
        <p>Entenda <br> o projeto</p>
    </header>
</template>

<script>
export default {
  name: 'HeaderBrand',
 
}
</script>

<style scoped>

header {
    display: flex;
    justify-content: space-between;
    padding-bottom: 1.4em;
}

header p:first-child {
    text-align: left;
}


</style>