<template>
  <PrimeiroComponente />
  <p>O dado da app é: {{ testando }}</p>
</template>

<script>
import { defineComponent } from "vue";
import PrimeiroComponente from "./components/PrimeiroComponente.vue";
export default defineComponent({
  name: "App",
  components: {
    PrimeiroComponente,
  },
  data() {
    return {
      testando: "teste",
    };
  },
});
</script>

<style lang="scss" scoped></style>
