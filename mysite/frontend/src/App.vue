<template>
  <div>
    <h2>This is a Vue 3 component!</h2>
    <button @click="increase">Clicked {{ count }} times.</button>
  </div>
</template>

<script lang="ts">
import { defineComponent, ref } from "vue";
export default defineComponent({
  setup() {
    const count = ref(0);
    const increase = () => {
      count.value++;
    };

    return {
      count,
      increase
    };
  }
});
</script>

<style scoped>
</style>