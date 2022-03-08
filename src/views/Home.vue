<template>
  <div class="home">
    <InicioComponent msg="Bienvenido al reproductor multimedia de MuniGT"/>
  </div>
</template>

<script>
// @ is an alias to /src
import InicioComponent from '@/components/Inicio.vue'

export default {
  name: 'Home',
  components: {
    InicioComponent
  }
}
</script>
