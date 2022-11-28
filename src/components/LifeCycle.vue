<template>
  <div>
    <h1>Meu nome é: {{ name }}</h1>
  </div>
</template>

<script>
import { defineComponent } from "@vue/runtime-core";

export default defineComponent({
  name: "LifeCycle",
  data() {
    return {
      name: "Ainda nao sei",
    };
  },
  created() {
    setTimeout(() => {
      this.name = "Farhan";
    }, 1000);
  },
  mounted() {
    setTimeout(() => {
      this.name = "Pedro";
    }, 3000);
  },
});
</script>

<style lang="scss" scoped></style>
