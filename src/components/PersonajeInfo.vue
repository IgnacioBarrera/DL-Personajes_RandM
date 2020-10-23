<template>
  <div class="imgfondo">
    <div v-for="(item, index) in datosRandM" :key="index">
    <img :src="item.image" alt=""> <span>{{item.name}}</span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'PersonajeInfo',
  props: {
    datosRandM: {
      type: Array,
      required: true
    }
  },
}
</script>

<style scoped>
  img {
    border-radius: 50%;
    width: 150px;
  }
  span {
    font-size: 50px;
    color: green;
  }
  .imgfondo{
    background-image: url('../assets/cropped-RM_page-header_background1-3.png');
    background-size: cover;
    background-repeat: no-repeat;
  }
</style>
