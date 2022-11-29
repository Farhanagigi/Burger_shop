<template>
  <PrimeiroComponente />
  <p>O dado da app é: {{ testando }}</p>
  <LifeCycle />
  <PessoaDesc />
</template>

<script>
import { defineComponent } from "vue";
import LifeCycle from "./components/LifeCycle.vue";
import PrimeiroComponente from "./components/PrimeiroComponente.vue";
import PessoaDesc from "./components/PessoaDesc.vue";

export default defineComponent({
  name: "App",
  components: {
    PrimeiroComponente,
    LifeCycle,
    PessoaDesc,
  },
  data() {
    return {
      testando: "teste",
    };
  },
});
</script>

<style lang="scss" scoped></style>
