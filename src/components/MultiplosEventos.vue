<template>
  <div>
    <button @click="primeiro(), segundo(), terceiro()">
      Activar multiplos Eventos
    </button>
    <p>{{ MultiplosEventos }}</p>
  </div>
</template>

<script>
import { defineComponent } from "@vue/runtime-core";

export default defineComponent({
  name: "MultiplosEventos",
  data() {
    return {
      MultiplosEventos: "",
    };
  },
  methods: {
    primeiro() {
      this.MultiplosEventos = "Primeiro Evento";
    },
    segundo() {
      setTimeout(() => {
        this.MultiplosEventos = "Segundo Evento";
      }, 2000);
    },
    terceiro() {
      setTimeout(() => {
        this.MultiplosEventos = "Terceiro Evento";
      }, 3500);
    },
  },
});
</script>

<style lang="scss" scoped></style>
