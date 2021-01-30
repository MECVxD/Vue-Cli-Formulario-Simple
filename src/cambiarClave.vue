<template>
  <div class="container">
    <div class="jumbotron">
      <mostrar-formulario>
        <!-- Si a una etiqueta no se le pone el atributo slot y tenemos definido un slot sin nombre, entonces la etiqueta será puesta en el
            slot sin nombre -->
        <h3 slot="titulo">Cambiar clave</h3>
        <div slot="elementos">
          <div class="col-auto">
            <label for="correo">Correo electrónico</label>
            <input type="email" class="form-control" placeholder="Escribe tu correo" id="correo">
          </div>
        </div>
        <div slot="boton" class="d-grid gap-2 col-6 mx-auto">
            <button class="btn btn-primary mb-3">Cambiar clave</button>
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