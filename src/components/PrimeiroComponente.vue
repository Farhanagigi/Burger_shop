<template>
  <div>
    <h1>Ola Vue!</h1>
    <p>Meu nome é: {{ name }} e trabalhou como {{ profissao }}</p>
  </div>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "PrimeiroComponente",
  data() {
    return {
      name: "Farhan",
      profissao: "Programador",
    };
  },
});
</script>

<style lang="scss" scoped></style>
