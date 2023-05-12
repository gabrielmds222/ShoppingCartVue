<script setup lang="ts">
import Produto from "./components/Produto.vue";

// export default {
//   name: 'App',

//   components: {
//    Produto,
//   },

//   data: () => ({
//     //
//   }),
// };
</script>

<template>
  <main class="pagina">
    <div class="container-titulo">
      <h1 class="titulo">Carrinho de compras</h1>
    </div>
    <div class="conteudo">
      <section>
        <Contagem />
        <table>
          <thead>
            <tr>
              <th colSpan="{4}"></th>
            </tr>
          </thead>
          <tbody>
            <Produto />
          </tbody>
        </table>
      </section>
      <aside>
        <Resumo />
      </aside>
    </div>
  </main>
</template>

<style scoped>
.pagina {
  display: flex;
  flex-direction: column;
  align-items: center;
  background-color: #eeeeee;
  padding: 0 30px 30px;
  height: 100vh;
  width: 100vw;
  margin: auto;
}

.container-titulo {
  margin-top: 40px;
}

.conteudo {
  display: flex;
  width: 90vw;
  flex-direction: row;
  margin-top: calc(2rem + 10px);
}

section {
  background-color: #fff;
  flex: 1;
  padding: 10px 40px;
}
table {
  width: 100%;
  border-collapse: collapse;
}

thead tr {
  border-bottom: 3px solid #eee;
}

thead th {
  text-align: left;
  padding-bottom: 10px;
  text-transform: uppercase;
  color: #666;
}

aside {
  background-color: #e0e0e0;
  width: 35%;
}
</style>
