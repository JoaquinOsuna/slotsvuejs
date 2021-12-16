<template>
  <div class="container">
    <div class="mt-4 p-5 bg-primary text-white rounded">
        <mostrar-formulario>
          <div slot="titulo"><h3>Iniciar sesion</h3></div>
           <div class="form-group" slot="elementos">
            <label for="">Correo Electronico</label>
            <input type="email" class="form-control" id="correo" placeholder="Escribe tu correo electronico">
            <label for="clave">Password</label>
            <input type="password" class="form-control" id="clave" placeholder="Escribe tu password">
            <br>
          </div>
          <div slot="boton"><button class="btn btn-danger">Iniciar sesion</button></div>
          
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
