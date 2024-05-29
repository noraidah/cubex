<template>
  <div>
    <h1 class="q-ma-lg">Products</h1>

    <main class="row justify-start item-center">
      <q-card
        v-for="product in products"
        :key="product.id"
        class="q-ma-lg my-card"
      >
        <q-img src="https://cdn.quasar.dev/img/parallax2.jpg">
          <div class="absolute-bottom">
            <div class="text-h6">{{ product.name }}</div>
            <div class="text-subtitle2">BND {{ product.price }}</div>
          </div>
        </q-img>

        <q-card-actions>
          <q-btn flat>Buy</q-btn>
        </q-card-actions>
      </q-card>
    </main>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const products = ref([
  {
    id: 1,
    name: 'Skateboard',
    price: 13.99,
  },
  {
    id: 2,
    name: 'Handbag',
    price: 43.99,
  },
  {
    id: 3,
    name: 'iPhone',
    price: 400.0,
  },
  {
    id: 4,
    name: 'Smart Watch',
    price: 130.99,
  },
  {
    id: 5,
    name: 'Apple',
    price: 1.99,
  },
  {
    id: 4,
    name: 'Smart Watch',
    price: 130.99,
  },
  {
    id: 5,
    name: 'Apple',
    price: 1.99,
  },
  {
    id: 6,
    name: 'Barang bagus',
    price: 99.99,
  },
]);
</script>

<style>
.my-card {
  width: 100%;
  max-width: 250px;
}
</style>
