<script setup lang="ts">
import { reactive } from 'vue';

type stylesClas = {
  btn: boolean;
  ['btn-color']: boolean;
};

const objectClass: stylesClas = reactive({
  btn: true,
  'btn-color': true,
});

const toggleClass = () => {
  objectClass.btn = !objectClass.btn;
  objectClass['btn-color'] = !objectClass['btn-color'];
};
</script>

<template>
  <button @click="toggleClass" :class="objectClass">clase dynamic</button>
</template>

<style scoped>
.btn {
  background: red;
}
.btn-color {
  color: black;
}
</style>
