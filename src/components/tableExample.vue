<template>
  <v-data-table
    :items="usuarios"
    :headers="cabecalhos"
    class="elevation-1"
  ></v-data-table>
</template>

<script>
import axios from "axios";

export default {
  name: "tableExample",
  data() {
    return {
      cabecalhos: [{ text: "Nome", value: "nome" }],
      usuarios: [],
    };
  },
  mounted() {
    axios.get("https://jsonplaceholder.typicode.com/users").then((response) => {
      this.usuarios = response.data.map((user) => ({ nome: user.name }));
    });
  },
};
</script>
