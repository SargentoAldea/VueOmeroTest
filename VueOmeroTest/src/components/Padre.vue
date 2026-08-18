<template>
  <div>
    <Hijo mensaje="Hola desde el padre" />

    <Hijo2 mensaje2="Hola desde el padre hijo2" />

    <Hijo3 mensaje3="Hola desde el padre hijo3" />
  </div>
  <div>
    <HijoBoton @saludo="mostrarSaludo" />
    <p v-if="mensaje">{{ mensaje }}</p>
  </div>
    
</template>
<script>
import Hijo from './Hijo.vue'
import Hijo2 from './Hijo2.vue'
import Hijo3 from './Hijo3.vue'
import HijoBoton from './HijoBoton.vue'

export default {
  components: {
    Hijo,
    Hijo2,
    Hijo3,
    HijoBoton
  },
  data(){
    return {mensaje: ''}
  },
  methods: {
    mostrarSaludo () {
      this.mensaje = 'Hola desde el hijo'
    }
  }
}

</script>