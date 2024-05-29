<template>
  <q-page>
    <product-list />
  </q-page>
</template>

<script setup lang="ts">
import ProductList from 'components/ProductList.vue';

defineOptions({
  name: 'IndexPage',
});
</script>
