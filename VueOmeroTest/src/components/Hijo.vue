<template>
  <div>
    <p>{{ mensaje }}</p>

    <Nieto1 mensaje4 ="Hola desde el padre Nieto1" />
  </div>
</template>

<script>
import Nieto1 from './Nieto1.vue'

export default {
  props: ['mensaje'],
  components: {
    Nieto1
  }
}
</script>