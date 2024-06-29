<script setup lang="ts">
import { type Ref, ref, computed } from 'vue';

const classBackGround: Ref<boolean> = ref(false);
const classColor: Ref<boolean> = ref(false);

const objectClass = computed(() => ({
  btn: classBackGround.value,
  ['btn-color']: classColor.value,
}));

const toggleClass = () => {
  classBackGround.value = !classBackGround.value;
  classColor.value = !classColor.value;
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
