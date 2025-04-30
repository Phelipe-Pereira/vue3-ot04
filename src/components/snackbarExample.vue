<template>
  <v-snackbar v-model="mostrarSnackbar" color="success">
    Ação realizada com sucesso!
    <template #actions>
      <v-btn text @click="mostrarSnackbar = false"> Fechar </v-btn>
    </template>
  </v-snackbar>
  <v-btn @Click="mostrarSnackbar = true"> Mostrar </v-btn>
</template>

<script>
export default {
  name: "snackbarExample",
  data() {
    return {
      mostrarSnackbar: false,
    };
  },
};
</script>
