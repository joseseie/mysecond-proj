<template>
  <div>
  <keep-alive>
    <component v-bind:is="component"></component>
    </keep-alive>
   <!-- <form-one></form-one> -->
    <button v-on:click="component = 'form-one'">Show Form One</button>
    <button v-on:click="component = 'form-two'">Show Form Two</button>
  </div>
</template>

<script>
import formOne from './components/formOne.vue'
import formTwo from './components/formTwo.vue'
export default {
  components:{
    'form-one': formOne,
    'form-two': formTwo
  },
  data () {
    return {
      component: 'form-one'
    }
  },
  methods:{

  }
}
</script>

<style>
div:last-child {
  padding: 10px;
}
</style>
