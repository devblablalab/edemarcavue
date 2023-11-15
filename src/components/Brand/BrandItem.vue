<template>
   <a  :href="link || '#'" class="brand-item" target="_blank">
      <p class="flex-1">{{ id + 1 }}</p>
      <p class="fw-bold flex-2">{{ price || 'R$ 0,00' }}</p>
      <p class="flex-2">{{ brand }}</p>
   </a>
</template>

<script>
export default {
  name: 'BrandItem',
  props: {
    id: Number,
    price: String,
    brand: String,
    link: String
  }
}
</script>

<style scoped>

.brand-item {
    display: flex;
    justify-content: space-around;
    align-items: center;
    gap: 1em;
    border-bottom: 2px dashed var(--muted);
    font-size: 1.3em;
    color: var(--muted);
    padding: 1em;
    transition: all .2s ease-in-out;
} 

.brand-item:hover {
  background-color: var(--muted);
  color: var(--light);
}

@media screen and (max-width:380px) {
  .brand-item {
    font-size: .9em;
  }
}
</style>