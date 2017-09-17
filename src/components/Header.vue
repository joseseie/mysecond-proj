<template>
  <header>
    <h1 v-on:click="changeTitle">{{title}}</h1>
  </header>
</template>

<script>
import {bus} from '../main';
export default {
  props:{
    title:{
      type: String
    }
  },
  data () {
    return {
      titleH: 'Jose Seie Vue no Header'
    }
  },
  methods:{
    changeTitle: function(){
      //this.$emit('changeTitle','Vue Wizard'); //Evento a ser acionado, e pode ser tratado no App.vue
      this.title = 'Vue Wizard';
      bus.$emit('titleChenged','Vue Wizard');
    }
  }
}
</script>

<style scoped>
header{
  background: lightgreen;
  padding: 10px;
}
h1 {
  color: #222;
  text-align: center;
}
</style>
