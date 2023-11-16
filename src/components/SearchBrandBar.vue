<template lang="">
  <input v-model="filter" @input="handleInput" placeholder="Filtrar por marca" />
</template>

<script>
    import { ref, watch, inject } from 'vue';

    export default {
        setup(props,{ emit }) {
            const filter = ref('');
            const brandsData  = inject('brandsData');

            const handleInput = () => {
                const filteredData = brandsData.value.filter(brand =>
                    brand.brand.toLowerCase().includes(filter.value.toLowerCase())
                );

                emit('filter-updated',filteredData);
            };

            watch(() => filter, handleInput);

            return {
                filter,
                handleInput,
            };
        }
    }
</script>

<style lang="">
    
</style>