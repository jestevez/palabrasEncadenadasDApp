<template>
  <div>
    <button v-on:click="sendContract">Generar nuevo número</button>
<h3>Introduce un número entre el 0 y el 4 y comprueba si has acertado el número secreto</h3>
<input v-model="numero" placeholder="introduce un número">
<button v-on:click="callContract">Enviar el número</button>
  </div>
</template>

<script>
import ethConfig from "../../config/ethConfig.js";

export default {
  name: "PalabrasEncadenadas",
  data() {
    return {
      numero: 0
    };
  },
  methods: {
    callContract() {
      alert("Número incorrecto");
    },

    sendContract() {
      alert("Nuevo número generado");
    }
  }
};
</script>

<style scoped>
h1,
h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}

button {
  background-color: #4caf50;
  border: none;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 4px 2px;
  cursor: pointer;
}
</style>
