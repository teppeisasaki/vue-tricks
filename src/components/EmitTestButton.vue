<template>
  <button v-on:click="clickHandler">Click me!</button>
</template>

<script>
  export default {
    methods: {
      clickHandler() {
        this.$emit("emitTrigger", "emitParam");
      }
    }
  }
</script>

<style scoped>

</style>
