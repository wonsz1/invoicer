<template>
  <div>
    <br>
    <b-form
      @submit="onSubmit">

      <b-form-group 
        id="emailGroup"
        label="Email"
        label-for="email" >
        
        <b-form-input 
          id="email"
          v-model="form.email"
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
      <b-form-group
        id="passwordConfirmGroup"
        label="Confirm"
        label-for="password-confirm">

        <b-form-input
          id="password-confirm"
          v-model="form.confirm"
          type="password"
          required/>
      </b-form-group>
      
      <b-button
        type="submit"
        variant="primary">Register</b-button>
    </b-form>
    <br>
    <nuxt-link to="/">Go back</nuxt-link>
  </div>
</template>

<script>
export default {
  data() {
    return {
      form: {
        email: '',
        password: '',
        confirm: ''
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