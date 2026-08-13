<template>
  <div>
    <p>{{ mensaje2 }}</p>

    <Nieto2 mensaje5 ="Hola desde el padre Nieto2" />
  </div>
</template>

<script>

import Nieto2 from './Nieto2.vue'

export default {
  props: ['mensaje2'],
  components: {
    Nieto2
  }
}
</script>