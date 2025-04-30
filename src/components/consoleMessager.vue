<template>
  <v-btn color="primary" @click="printMessage">Print Message</v-btn>
</template>

<script>
export default {
  name: "ConsoleMessager",
  methods: {
    printMessage() {
      console.log("Printing message");
    },
  },
};
</script>
