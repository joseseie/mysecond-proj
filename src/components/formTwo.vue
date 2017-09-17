<template>
  <div>
   <form-helper>
     <div slot="form-header">
       <h3>Form Two- Log In</h3>
       <p>Enter you details to log-in</p>
     </div>
     <div slot="form-fields">
       <input type="text" placeholder="username" required>
       <input type="password" placeholder="password" required>
     </div>
     <div slot="form-controls">
      <button v-on:click="handleSubmit">Login</button>
     </div>

   </form-helper>

  </div>
</template>

<script>
import formhelper from './components/form-helper.vue'
export default {
  components:{
    'form-helper': formhelper
  },
  data () {
    return {
      
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
