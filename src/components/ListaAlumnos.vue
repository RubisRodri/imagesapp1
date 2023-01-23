<template>
  <div>
    
    <CardList
    :lista="lista"
     />
  </div>
</template>

<script>
import CardList from '@/components/CardList.vue'

export default {
    name:'ListaAlumnos',
    components:{
        CardList
    },
    data(){
        return{
            lista:[
                {
                nombre:'Esteban',
                materia:'matematicas',
                carro:'ferrary',
                id: '01'
                },
                {
                nombre:'Ronny',
                materia:'matematicas',
                carro:'autobus',
                id:'02'
                },
                {
                nombre:'eduardo',
                materia:'matematicas',
                carro:'mercedes',
                id:'03' 
                }
            ]
        }
    }
}
</script>

<style>

</style>