<template>
  <div>
    <h2>Esta é a descricao da pessoa: {{ name }}</h2>
    <InfoR />

    <FormLario />
  </div>
</template>

<script>
import { defineComponent } from "@vue/runtime-core";
import InfoR from "./InfoR.vue";
import FormLario from "./FormLario.vue";

export default defineComponent({
  name: "PessoaDesc",
  components: {
    InfoR,
    FormLario,
  },
  data() {
    return {
      name: "Farhan",
    };
  },
});
</script>

<style lang="scss" scoped></style>
