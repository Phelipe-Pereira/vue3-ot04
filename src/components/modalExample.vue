<template>
  <div>
    <v-btn color="primary" @click="modalAberto = true">Abrir Modal</v-btn>

    <v-dialog v-model="modalAberto" max-width="500">
      <v-card>
        <v-card-title>Título do Modal Exemplo</v-card-title>
        <v-card-text>Este é o conteúdo do modal.</v-card-text>
        <v-card-actions>
          <v-spacer></v-spacer>
          <v-btn color="secondary" @click="modalAberto = false">Fechar</v-btn>
        </v-card-actions>
      </v-card>
    </v-dialog>
  </div>
</template>

<script>
export default {
  name: "modalExample",
  data() {
    return {
      modalAberto: false,
    };
  },
};
</script>
