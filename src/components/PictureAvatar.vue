<template>
  <div>
    <img :src="avatar" :alt="descricao" />
    <MudarImagem @mudarImagem="trocaravatar" />
  </div>
</template>

<script>
import { defineComponent } from "@vue/runtime-core";
import MudarImagem from "./MudarImagem.vue";

export default defineComponent({
  name: "PictureAvatar",
  components: {
    MudarImagem,
  },
  data() {
    return {
      avatar: "../img/icons8-customer-100.png/",
      descricao: "Farhan Agigi",
    };
  },
  methods: {
    trocaravatar() {
      this.avatar = "./img/male.png";
      this.descricao = "Outro Usuario";
    },
  },
});
</script>

<style lang="scss" scoped></style>
