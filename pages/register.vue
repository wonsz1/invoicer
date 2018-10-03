<template>
  <section class="container">
    <div>
      <h1 class="title">
        fakturownik
      </h1>
      <register-form/>
    </div>
  </section>
</template>

<script>
  import registerForm from '~/components/register_form.vue';
  
  export default {
    components: {
      registerForm
    }
  }
</script>