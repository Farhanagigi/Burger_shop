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

    <div>
      <button @click="showEmail">{{ textoBotao }}</button>
    </div>
    <p v-show="mostrar_email">Mande uma mensagem para : {{ name }}</p>
    <p>
      Para acessar o meu portfolio
      <a v-bind:href="meu_link" target="_blank">basta clicar aqui</a>
    </p>
    <PictureAvatar />
  </div>
</template>

<script>
import { defineComponent } from "vue";
import PictureAvatar from "./PictureAvatar.vue";

export default defineComponent({
  name: "InfoR",
  components: {
    PictureAvatar,
  },
  data() {
    return {
      esta_trabalhando: true,
      mostrar_email: false,
      name: "Farhan@email.com",
      meu_link: "https://www.google.com",
      textoBotao: "Mostrar Email",
    };
  },
  methods: {
    showEmail() {
      this.mostrar_email = !this.mostrar_email;
      if (!this.mostrar_email) {
        this.textoBotao = "Mostrar Email";
      } else {
        this.textoBotao = "Esconder Email";
      }
    },
  },
});
</script>

<style lang="scss" scoped></style>
