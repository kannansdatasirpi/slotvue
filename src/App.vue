<template>
  <div id="form-help">
    <form-helper>
      <template v-slot:form-header>
        <h3>This is the title of the form</h3>
        <p>Information about the form</p>
      </template> 
      <template v-slot:form-fields>
        <input type="text" placeholder="name" required />
        <input type="password" placeholder="password" required />
      </template> 
      <template v-slot:form-controls>
        <button @click="handleSubmit">Submit</button>
      </template>
    </form-helper>
  </div>
  
</template>

<script>
import formHelper from './components/formHelper.vue'

export default {
  
  components: {
    'form-helper': formHelper
  },
  data() {
    return {

    }
  },
  methods: {

  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
