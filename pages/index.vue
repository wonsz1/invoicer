<template>
  <section class="container">
    <div>
      <logo/>
      <h1 class="title">
        fakturownik
      </h1>
      <h2 class="subtitle">
        My great Nuxt.js project
      </h2>
      <div>
        <login-form/>
      </div>
    </div>
  </section>
</template>

<script>
import Logo from '~/components/Logo.vue'
import LoginForm from '~/components/login_form.vue'

export default {
  components: {
    LoginForm, Logo
  }
}
</script>

<style>

.container {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
