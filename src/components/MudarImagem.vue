<template>
  <div>
    <button @click="$emit('mudarImagem')">Trocar Imagem do perfil</button>
  </div>
</template>

<script>
import { defineComponent } from "@vue/runtime-core";

export default defineComponent({
  name: "MudarImagem",
  emits: ["mudarImagem"],
});
</script>

<style lang="scss" scoped></style>
