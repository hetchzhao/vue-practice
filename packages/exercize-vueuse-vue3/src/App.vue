<template>
  <div id="app">
    <span>x: {{ x }}</span>
    <span>y: {{ y }}</span>
  </div>
</template>

<script>
import { useMouse } from "@vueuse/core";

export default {
  setup() {
    const { x, y } = useMouse();

    return {
      x,
      y,
    };
  },
};
</script>

<style scoped></style>
