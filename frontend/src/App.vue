

<template>
  <h1>bonjour</h1>
  <checkbox label="bonjour"
  @check="console.log('couche')"
  @uncheck="console.log('decoucjer')"/>
</template>

<script setup>
import checkbox  from './components/checkbox.vue';
</script>

<style scoped></style>
