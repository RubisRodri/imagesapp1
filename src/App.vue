<template>
  <v-app>
    <navbar-header></navbar-header>
    <v-main>
      <!-- <lista-alumnos></lista-alumnos>
      <listamaterias></listamaterias> -->
    

    <a @click="mostrarComponente(materias)">materias</a>
    <v-btn @click="mostrarComponente(alumnos)">Biologia</v-btn>

    <lista-alumnos></lista-alumnos>
    <component :is="componentSelect" />
    </v-main>
  </v-app>
</template>





<script>
import NavbarHeader from '@/components/NavbarHeader.vue';
import ListaAlumnos from '@/components/ListaAlumnos.vue';
import Listamaterias from '@/components/Listamaterias.vue'



 export default {
      name: 'App',
      data() {
          return {
            materias : Listamaterias,
            alumnos : ListaAlumnos,
            componentSelect: null
          }
      },
      components : {
        NavbarHeader,
        ListaAlumnos,
        Listamaterias
      },
      methods: {
        mostrarComponente: function (componente){
          this.componentSelect = componente
        }
      }
 }
</script>

<style>
</style>




