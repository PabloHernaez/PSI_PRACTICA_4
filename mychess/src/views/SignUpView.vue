<template>
  <div>
    <div>
      <!-- <img></img> @signup-user="handleSignUp" Aqui es donde introduciremos la imagen del componente -->
    </div>
    <div>
      <sign-up-form @signup-user="handleSignUp" />
    </div>
  </div>
</template>

<script>
import "../components/SignUpForm.vue";
import SignUpForm from "../components/SignUpForm.vue";

export default {
  name: "signup-view",
  components: {
    SignUpForm,
  },

  setup() {},

  methods: {
    handleSignUp(message) {
      console.log(message);
      //Aqui es donde introduciremos el apartado de tener registrado el token en la aplicacion
    },
  },
};
</script>
