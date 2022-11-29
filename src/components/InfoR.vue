<template>
  <div>
    <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
    <p v-else>Estou em busca de novas oportunidades</p>
    <p>Utilizo as seguintes tecnologias</p>
    <ul>
      <li>Javascript</li>
      <li>Java</li>
      <li>Vue</li>
    </ul>
    <p v-show="mostrar_email">Mande uma mensagem para : {{ name }}</p>
  </div>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "InfoR",
  data() {
    return {
      esta_trabalhando: true,
      mostrar_email: true,
      name: "Farhan@email.com",
    };
  },
});
</script>

<style lang="scss" scoped></style>
