<template>
  <div class="container">
    <div class="mt-4 p-5 bg-primary text-white rounded">
          <button class="btn btn-danger" @click="componenteSeleccionado = 'iniciarSesion'">Iniciar Sesion</button>
          <button class="btn btn-danger" @click="componenteSeleccionado = 'cambiarClave'">Cambiar password</button>

          <keep-alive>
            <component :is="componenteSeleccionado"></component>
          </keep-alive>  
    </div>
  </div>
</template>

<script>
import MostrarFormulario from './mostrarformulario.vue'
import IniciarSesion from './iniciarsesion.vue'
import CambiarClave from './cambiarclave.vue'
export default {
  components:{
    mostrarFormulario: MostrarFormulario,
    iniciarSesion: IniciarSesion,
    cambiarContra: CambiarClave,
  },
  data(){
      return{
        componenteSeleccionado: 'iniciarSesion'
      }
  }
}
</script>

<style scoped>
  h3{
    color: red;
  }
</style>
