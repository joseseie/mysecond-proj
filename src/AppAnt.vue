<template>
  <div>
  <!--
    <app-header v-bind:title="title" v-on:changeTitle="updateTitle($event)"></app-header>
    <!-- Com o v-bind:ninjas Estamos a dizer que queremos pegar os objectos 'ninjas' declarados no data e passar  para o componente app-ninja 
    <app-ninjas v-bind:ninjas="ninjas"></app-ninjas>
    <app-footer v-bind:title="title"></app-footer> -->
  <div>
  </div>
</template>

<script>
// import Ninjas from './Ninja.vue'
// import Header from './components/Header.vue'
// import Footer from './components/Footer.vue'
// import Ninjas from './components/Ninjas.vue'
import formhelper from './components/form-helper.vue'

export default {
  components:{
    // 'app-header': Header,
    // 'app-footer': Footer,
    // 'app-ninjas': Ninjas,
    'form-helper': formhelper
  },
  data () {
    return {
      ninjas: [
        {name: 'Hose',speciality: 'Jose Seie',show: false},
        {name: 'Jose Seie',speciality: 'Teste Vuw',show: false},
        {name: 'Mario Tanjo',speciality: 'Click Events',show: false},
        {name: 'Tango',speciality: 'Conditionals',show: false},
        {name: 'Kami',speciality: 'WebPack',show: false},
        {name: 'Yoshi',speciality: 'Data Diggin',show: false},
      ],
      // title:'Vue Seie JS'
      
    }
  },
  methods:{
    updateTitle:function(updateTitle){
      this.title = updateTitle;
    }
  }
}
</script>

<style scoped>

</style>
