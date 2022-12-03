<template>
  <h1>Hello, {{ val }}!</h1>
  <EmitTestButton v-on:emitTrigger="eventHandler">Click Me!</EmitTestButton>
</template>

<script>
  import EmitTestButton from "./components/EmitTestButton.vue";

  export default {
    components: {
      EmitTestButton
    },
    data() {
      return {
        val: "TEST",
      };
    },
    methods: {
      eventHandler(val) {
        this.val = val;
      }
    }
  }
</script>

<style scoped>
</style>
