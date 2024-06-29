<script setup lang="ts">
import { type Ref, ref } from 'vue';

const IsactiveClass: Ref<boolean> = ref(false);

const activeCalss = () => (IsactiveClass.value = !IsactiveClass.value);
</script>

<template>
  <button @click="activeCalss" :class="{ btn: IsactiveClass }">
    clase dynamic
  </button>
</template>

<style scoped>
.btn {
  background: red;
}
</style>
