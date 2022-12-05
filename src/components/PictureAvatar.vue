<template>
  <div>
    <img :src="avatar" :alt="descricao" />
  </div>
</template>

<script>
import { defineComponent } from "@vue/runtime-core";

export default defineComponent({
  name: "PictureAvatar",
  data() {
    return {
      avatar: "./img/icons8-customer-100.png",
      descricao: "Farhan Agigi",
    };
  },
});
</script>

<style lang="scss" scoped></style>
