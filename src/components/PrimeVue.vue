<script setup>

import Message from 'primevue/Message';
import Panel from 'primevue/panel';
import DataTable from 'primevue/datatable';
import Column from 'primevue/column';

const products = [
  {
    id: '1000',
    code: 'f230fh0g3',
    name: 'Bamboo Watch',
    description: 'Product Description',
    image: 'bamboo-watch.jpg',
    price: 65,
    category: 'Accessories',
    quantity: 24,
    inventoryStatus: 'INSTOCK',
    rating: 5
  },
  {
    id: '1001',
    code: 'iorqwe-089',
    name: 'Bamboo Watch 2',
    description: 'Product Description 2',
    image: 'bamboo-watch.jpg',
    price: 165,
    category: 'Accessories',
    quantity: 4,
    inventoryStatus: 'INSTOCK',
    rating: 4
  }
];

</script>

<template>
  <div class="container-fluid">
    <h3>PrimeVue</h3>
    <Message>PrimeVue</Message>
    <Panel header="Header">
      <p class="m-0">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore
        magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
        consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla
        pariatur.
        Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
      </p>
    </Panel>


    <DataTable :value="products" tableStyle="min-width: 50rem;">
      <Column field="code" header="Code" sortable style="width: 15%;"></Column>
      <Column field="name" header="Name" sortable></Column>
      <Column field="category" header="Category" sortable style="width: 15%"></Column>
      <Column field="quantity" header="Quantity" sortable style="width: 15%"></Column>
    </DataTable>
  </div>

</template>

<style scoped></style>
