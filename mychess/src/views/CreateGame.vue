<script>
export default {
  name: "createGame",

  setup() {
    const state = {
      joining: false,
    };
  },

  methods: {
    createGame() {
      //Aqui desataremos la lógica de que se nos cree el jueguito
    },

    joiningGame() {
      //Aqui desencadenaremos el evento que nos hará que se nos una a una sala concreta
    },
  },
};
</script>

<template>
  <div>
    <p>Presione para crear una partida</p>
    <input type="button" onclick="" value="CREATE GAME" />
    <p>Presione para unirse a una partida:</p>
    <input type="button" onclick="" value="JOIN GAME" />
  </div>
</template>
