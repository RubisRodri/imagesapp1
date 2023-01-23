<template>
  <div>
    <ul class="lista">
      <li
       class="lista-item"
       v-for="element in lista" :key="element.id">
        {{ element.nombre }}
        {{ element.materia }}
       
      </li>
    </ul>
  </div>
</template>

<script>
export default {
    name: 'CardList',
    props: {
        lista: Array
    }
}
</script>

