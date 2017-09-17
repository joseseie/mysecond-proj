<template>
<div>
<h1>Lista de Ninjas</h1>
  <ul>
    <li v-for="ninja in ninjas">{{ninja}}</li> 
  </ul>
  </div>
</template>

<script>
export default {
  data () {
    return {
      ninjas: ['Hose','Jose Seie','HYSn']
    }
  }
}
</script>

<style scoped>
h1{
    color: green;
  }
</style>
