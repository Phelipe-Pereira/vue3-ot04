<template>
  <v-app>
    <v-main>
      <v-container>
        <img alt="Vue logo" src="./assets/logo.png">
        <CardExample></CardExample>
        <ConsoleMessager></ConsoleMessager>
        <ModalExample></ModalExample>
        <SnackbarExample></SnackbarExample>
        <TableExample></TableExample>
        <ToolbarExample></ToolbarExample>
        <GridLayout></GridLayout>
        <LoginExample></LoginExample>
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
import CardExample from './components/cardExample.vue';
import ConsoleMessager from './components/consoleMessager.vue';
import GridLayout from './components/grid.vue'
import LoginExample from './components/loginExample.vue';
import ModalExample from './components/modalExample.vue';
import SnackbarExample from './components/snackbarExample.vue';
import TableExample from './components/tableExample.vue';
import ToolbarExample from './components/toolbarExample.vue';

export default {
  name: 'App',
  components: {
    GridLayout,
    CardExample,
    ConsoleMessager,
    ModalExample,
    SnackbarExample,
    TableExample,
    ToolbarExample,
    LoginExample
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
