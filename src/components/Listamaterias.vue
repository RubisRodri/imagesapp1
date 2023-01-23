<template>
<div class="curso">
   
    <CardList
    :lista="lista"
     />
</div>
</template>

<script>
import CardList from '@/components/CardList.vue';

export default {
    name:'Listamaterias',
    components:{
        CardList,
    },
    data(){
        return{
            lista:[
                {
                nombre:'Rubis',
                materia:'matematicas',
                img:'src:"@/assets/logo.png"',
                id: '01'
                },
                {
                nombre:'Ronny',
                materia:'biologia',
                id:'02'
                },
                {
                nombre:'eduardo',
                materia:'ciencias',
                id:'03'
                }
            ]
        }
    },

}
</script>

<style>

</style>