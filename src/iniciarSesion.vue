<template>
  <div class="container">
    <div class="jumbotron">
      <mostrar-formulario>
        <h3 slot="titulo">Iniciar sesión</h3>
        <div slot="elementos">
          <div class="col-auto">
            <label for="correo">Correo electrónico</label>
            <input type="email" class="form-control" placeholder="Escribe tu correo" id="correo">
          </div>
          <div class="col-auto">
            <label for="clave">Contraseña</label>
            <input type="password" class="form-control" id="clave" placeholder="Escribe tu contraseña">
          </div>
        </div>
        <div slot="boton" class="d-grid gap-2 col-6 mx-auto">
            <button class="btn btn-primary mb-3">Iniciar sesión</button>
        </div>
      </mostrar-formulario>
    </div>
  </div>
</template>

<script>
import MostrarFormulario from './mostrarFormulario.vue'
export default {
  components: {
    mostrarFormulario:MostrarFormulario
  }
}
</script>
