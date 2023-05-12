<script lang="ts">
// import { PhTrash } from "@phosphor-icons/vue";
export default {
  name: "Produto",

  data: () => ({
    //
  }),
};
</script>

<template>
  <tr>
    <td>
      <div class="produto-container">
        <img src="../../assets/ghostoftsushima.jpg" />
        <div class="infos">
          <div class="nome">Pizza</div>
          <div class="descricao">pizza 1</div>
          <div class="preco">R$ 100,00</div>
        </div>
      </div>
    </td>
    <td>
      <div class="qty">
        <input type="number" />
      </div>
    </td>
    <td>R$ 100,00</td>
    <td>
      <button>EXCLUIR</button>
    </td>
  </tr>
</template>

<style scoped>
tr {
  border-bottom: 3px solid #eee;
}

td {
  padding: 20px 0;
}
.produto-container {
  display: flex;
  align-items: center;
}

img {
  width: 100px;
  height: 100px;
}

.infos {
  margin-left: 20px;
}

.nome {
  font-size: 24px;
  font-weight: bold;
}

.descricao {
  width: 450px;
  font-size: 14px;
}
</style>
