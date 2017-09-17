<template>

  <div>
      <h1>Meu primeiro texto</h1>
      <ninja-seie></ninja-seie>
  </div>
</template>

<script>
import Ninjas from './Ninja.vue'

export default {
  components:{
    'ninja-seie': Ninjas
  },
  data () {
    return {
      title: 'Second vue project'
    }
  },
  methods:{

  }
}
</script  scoped>

<style>
  h1{
    color: red;
  }
</style>
