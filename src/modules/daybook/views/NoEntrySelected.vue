<template>
  <div class="d-flex justify-content-center">
      <h1 class="align-self-center">No hay nada selecciodado</h1>
  </div>
  <Fab/>
</template>

<script>
import { defineAsyncComponent } from 'vue'
export default {
    components: {
        Fab: defineAsyncComponent(() => import(/* webpackChunkName: "Fab" */ '../components/Fab.vue'))
    }
}
</script>

<style lang="scss" scoped>

    div{
        height: 100%;
    }

</style>