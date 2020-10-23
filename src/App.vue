<template>
  <div id="app">
    <PersonajeInfo :datosRandM="datosRandM" />
  </div>
</template>

<script>
import PersonajeInfo from './components/PersonajeInfo.vue'

export default {
  name: 'App',
  components: {
    PersonajeInfo
  },
  data() {
    return {
      datosRandM: [
        {name: 'Rick Sanchez', image: 'https://rickandmortyapi.com/api/character/avatar/1.jpeg'},  
        {name: 'Morty Smith', image: 'https://rickandmortyapi.com/api/character/avatar/2.jpeg'},  
        {name: 'Summer Smith', image: 'https://rickandmortyapi.com/api/character/avatar/3.jpeg'},  
        {name: 'Beth Smith', image: 'https://rickandmortyapi.com/api/character/avatar/4.jpeg'},  
        {name: 'Jerry Smith', image: 'https://rickandmortyapi.com/api/character/avatar/5.jpeg'},  
      ]
    }
  },
}
</script>

<style>
#app {
  margin: 0 auto;
}
</style>
