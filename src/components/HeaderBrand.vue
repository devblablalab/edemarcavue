<template>
    <header>
        <a class="header-item" href="#" target="_blank">por <br> BlaBlaLab</a>
        <p class="header-item">Entenda <br> o projeto</p>
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

header .header-item {
    color: var(--muted);
    transition: all .2s;
    cursor: pointer;
}

header .header-item:hover {
    color: var(--dark);
}

header p:first-child {
    text-align: left;
}
</style>