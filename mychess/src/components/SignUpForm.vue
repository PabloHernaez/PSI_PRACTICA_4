<template>
  <div>
    <form @submit.prevent="enviarFormulario">
      <!-- @submit.prevent="enviarFormulario"-->
      <p>Introduzca aqui el usuario:</p>
      <br />
      <input type="text" placeholder="Usuario" v-model="user.name" />
      <p>Introduzca aqui la contraseña:</p>
      <br />
      <input type="password" placeholder="Contraseña" v-model="user.password" />
      <input type="submit" />
    </form>
  </div>
</template>

<script>
import { ref } from "vue";

export default {
  name: "sign-up-form",
  setup() {
    const user = ref({
      name: "Pablo",
      password: "Password",
    });

    return {
      user,
    };
  },

  methods: {
    enviarFormulario() {
      //Aqui llevariamos a cabo la lógica del register

      this.$emit("signup-user", this.user);
    },
  },
};
</script>
