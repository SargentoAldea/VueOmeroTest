<template>
  <div>
    <p>{{ mensaje3 }}</p>

    <Nieto3 mensaje6 ="Hola desde el padre Nieto3" />
  </div>
</template>

<script>

import Nieto3 from './Nieto3.vue'

export default {
  props: ['mensaje3'],
  components: {

    Nieto3

  }
}
</script>