<template>
  <div>
    <h2>Minha lista de itens:</h2>
    <ul>
      <li v-for="(item, index) in listaDeItens" :key="index">{{ item }}</li>
    </ul>
  </div>
</template>

<script lang="ts">
export default {
  data() {
    return {
      listaDeItens: {
        item1: "Item 1",
        item2: "Item 2",
        item3: "Item 3",
        item4: "Item 4",
      },
    };
  },
};
</script>
