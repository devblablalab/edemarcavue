<template>
    <ul class="brand-list">
        <BrandItem 
            v-for="(item,index) in brands" 
            :key="index" 
            :id="index"
            :brand=item.brand 
            :price="item.price"
            :link="item.link"
        />
    </ul>
</template>

<script>
    import data from '../../../data.json'
    import BrandItem from './BrandItem.vue';
    export default {
        data() {
            return {
                brands: data
            };
        },
        components: { BrandItem }
    }
</script>

<style scoped>
    .brand-list {

    }
</style>