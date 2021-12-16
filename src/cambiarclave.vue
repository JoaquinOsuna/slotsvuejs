<template>
  <div class="container">
    <div class="mt-4 p-5 bg-primary text-white rounded">
        <mostrar-formulario>
          <div slot="titulo"><h3>Cambiar Password</h3></div>
           <div class="form-group" slot="elementos">
            <label for="">Correo Electronico</label>
            <input type="email" class="form-control" id="correo" placeholder="Escribe tu correo electronico">
            <br>
          </div>
          <div slot="boton"><button class="btn btn-danger">Cambiar clave</button></div>
          
        </mostrar-formulario>
    </div>
  </div>
</template>

<script>
import MostrarFormulario from './mostrarformulario.vue'
export default {
  components:{
    mostrarFormulario: MostrarFormulario
  },
  data(){

  }
}
</script>

<style scoped>
  h3{
    color: red;
  }
</style>
