<template>
  <div>
   <form-helper>
     <div slot="form-header">
       <h3>Form One - Contact Us/h3>
       <p>Fill in this form to contact us</p>
     </div>
     <div slot="form-fields">
       <input type="text" placeholder="name" required>
       <label>You message:</label>
       <textarea></textarea>
     </div>
     <div slot="form-controls">
      <button v-on:click="handleSubmit">Send</button>
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
      title: 'I am the slot title dina,oc'
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
