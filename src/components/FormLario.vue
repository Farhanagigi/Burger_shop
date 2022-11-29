<template>
  <div>
    <h2>Meu Formulario:</h2>
    <form action="">
      <div>
        <InputText />
      </div>

      <div>
        <InputText />
      </div>

      <div>
        <SubmitButton />
      </div>
    </form>
  </div>
</template>

<script>
import { defineComponent } from "@vue/runtime-core";
import InputText from "./Form/InputText.vue";
import SubmitButton from "./Form/SubmitButton.vue";

export default defineComponent({
  name: "FormLario",
  components: {
    InputText,
    SubmitButton,
  },
});
</script>

<style lang="scss" scoped></style>
