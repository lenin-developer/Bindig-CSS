<script setup lang="ts">
import HelloWorld from './components/HelloWorld.vue';
import BtnClassSimple from './components/BtnClassSimple.vue';
import BtnClassDynamic from './components/BtnClassDynamic.vue';
import BtnObjetoClass from './components/BtnObjetoClass.vue';
import BtnClassComputed from './components/BtnClassComputed.vue';
</script>

<template>
  <HelloWorld />
  <h2>propiedad class</h2>
  <BtnClassSimple />
  <h2>propiedad :class</h2>
  <BtnClassDynamic />
  <h2>reactive object class</h2>
  <BtnObjetoClass />
  <h2>computed class</h2>
  <BtnClassComputed />
</template>

<style scoped></style>
