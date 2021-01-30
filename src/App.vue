<template>
  <div class="container">
    <div class="jumbotron">
      <button class="btn btn-primary" @click="componenteSeleccionado= 'IniciarSesion'">Iniciar sesión</button>
      <button class="btn btn-primary" @click="componenteSeleccionado= 'CambiarClave'">Cambiar contraseña</button>
      <hr>
      <keep-alive>
        <component :is="componenteSeleccionado"></component>
      </keep-alive>
    </div>
  </div>
</template>

<script>
import IniciarSesion from './iniciarSesion.vue'
import CambiarClave from './cambiarClave.vue'
export default {
  components: {
    IniciarSesion,
    CambiarClave
  },
  data() {
    return {
      componenteSeleccionado: 'IniciarSesion'
    }
  }
}
</script>

<style>
</style>

