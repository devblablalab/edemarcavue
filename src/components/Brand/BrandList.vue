<template>
    <SearchBrandBar @filter-updated="handleFilterUpdated" />
    <ul class="brand-list">
        <BrandItem 
            v-for="(item,index) in brandsData" 
            :key="index" 
            :id="index"
            :brand=item.brand 
            :price="item.price"
            :link="item.link"
        />
    </ul>
</template>

<script>
    import { ref, provide, onMounted } from 'vue';
    import data from '../../../data.json';
    import BrandItem from './BrandItem.vue';
    import SearchBrandBar from '../SearchBrandBar.vue';

    export default {
        setup() {
            const brandsData = ref([]);

            onMounted(() => {
                brandsData.value = data
            }),

            provide('brandsData', brandsData);

            const handleFilterUpdated = filteredData => {
                brandsData.value = filteredData;
            };

            return {
                brandsData,
                handleFilterUpdated
            }
        },
        components: { BrandItem, SearchBrandBar }
    }
</script>

<style scoped>  

</style>