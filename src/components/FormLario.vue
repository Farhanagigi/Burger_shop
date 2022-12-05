<template>
  <div>
    <h2>Meu Formulario:</h2>
    <form action="" @submit="enviarFormulario($event)">
      <div>
        <input type="text" v-model="name" />
        <!-- <InputText /> -->
      </div>

      <div>
        <input type="text" v-model="email" />
        <!-- <InputText /> -->
      </div>

      <div>
        <SubmitButton />
      </div>
    </form>
  </div>
</template>

<script>
import { defineComponent } from "@vue/runtime-core";
/* import InputText from "./Form/InputText.vue"; */
import SubmitButton from "./Form/SubmitButton.vue";

export default defineComponent({
  name: "FormLario",
  components: {
    /* InputText, */
    SubmitButton,
  },
  data() {
    return {
      name: "",
      email: "",
    };
  },
  methods: {
    enviarFormulario(e) {
      e.preventDefault();

      const name = this.name;
      const email = this.email;

      console.log("Nome: " + name);
      console.log("Email: " + email);
      console.log("Formulario Enviado!");

      //AJAX

      //Inserir os dados do banco
    },
  },
});
</script>

<style lang="scss" scoped></style>
