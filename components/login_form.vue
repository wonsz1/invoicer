<template>
  <div>
    <br>
    <b-form
      @submit="onSubmit">

      <b-form-group 
        id="loginGroup"
        label="Login"
        label-for="login" >
        
        <b-form-input 
          id="login"
          v-model="form.login"
          type="text"
          required/>
      </b-form-group>

      <b-form-group
        id="passwordGroup"
        label="Password"
        label-for="password">

        <b-form-input
          id="password"
          v-model="form.password"
          type="password"
          required/>
      </b-form-group>
      
      <b-button
        type="submit"
        variant="primary">Submit</b-button>
    </b-form>
    <br>
  </div>
</template>

<script>
export default {
  data() {
    return {
      form: {
        login: '',
        password: ''
      }
    }
  },
  methods: {
    onSubmit(e) {
      e.preventDefault();
      alert(JSON.stringify(this.form));
    }
  }
}
</script>