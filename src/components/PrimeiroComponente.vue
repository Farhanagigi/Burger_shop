<template>
  <div>
    <h1>Ola Vue!</h1>
    <p>Meu nome é: {{ name }} e trabalhou como {{ profissao }}</p>
  </div>
  <MultiplosEventos />
</template>

<script>
import { defineComponent } from "vue";
import MultiplosEventos from "./MultiplosEventos.vue";

export default defineComponent({
  name: "PrimeiroComponente",
  components: {
    MultiplosEventos,
  },
  data() {
    return {
      name: "Farhan",
      profissao: "Programador",
    };
  },
});
</script>

<style lang="scss" scoped></style>
