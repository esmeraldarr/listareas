<template>
  <div id="app" class="container">
    <div class="jumbotron">
      <titulo :titulo="titulo"></titulo>
      <nueva-tarea v-bind:tareas="tareas"></nueva-tarea>
      <lista-tarea :listaT="listaT"></lista-tarea>
    </div>
  </div>
</template>

<script>
import Titulo from './Titulo.vue'
import NuevaTarea from './nuevaTarea.vue'
import ListaTareas from './listaTareas.vue'
export default {
    components: {
        Titulo,
        NuevaTarea,
        ListaTareas
    },
    data(){
        return {
            titulo: 'lista de tareas',
            tareas: [
            {
              texto: 'Aprender Vue.js',
              terminada: false
            },
            {
              texto: 'Aprender Angular 2',
              terminada: false
            },
            {
              texto: 'Aprender Ionic 2',
              terminada: false
            }
          ]
        }
    }
}
</script>

<style>

</style>
