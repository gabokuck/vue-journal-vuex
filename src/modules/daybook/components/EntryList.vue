<template>
  <div class="entry-list-container">
    <div class="PX-2 PT-2">
        <input 
        type="text"
        class="form-control"
        placeholder="Buscar entrada"
        >
        <div class="entry-scrollarea">
          <h2 v-for="item of 100" :key="item">
            <Entry/>
          </h2>
        </div>
    </div>
  </div>
</template>

<script>
import { defineAsyncComponent } from 'vue'

export default {  
  components: {
    Entry: defineAsyncComponent(() => import(/* webpackChunkName: "Entry" */ '../components/Entry.vue'))
  }
}
</script>

<style lang="scss" scoped>

  .entry-list-container{
    border-right: 1px solid #2c3e50;
    height: calc(100vh - 56px);
  }

  .entry-scrollarea{
    height: calc(100vh - 100px);
    overflow: scroll;
  }

</style>