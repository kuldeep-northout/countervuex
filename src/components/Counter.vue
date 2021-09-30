<template>
<div>
  <h2>Counter</h2>
  <h1>{{counter}}</h1>
  <div class="btn-group"> </div>
  <button class="btn-group-item" @click="increment">+</button>
  <button class="btn-group-item"  @click="decrement">-</button>

</div>

</template>

<script>
import {mapGetters,mapActions} from "vuex"
export default {
    computed:{
      ...mapGetters([
        'counter'
      ])
    },
    methods:{
      ...mapActions([
        'increment',
        'decrement'
      ])
    }
}
</script>

<style>

</style>