<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    
    <form @submit.prevent="submitForm()">
      <BaseInput label="First Name" name="firstName"  />
      <BaseInput label="Last Name" name="lastName" />
      <BaseInput label="Email" name="email" />
    </form>

    <pre>{{ this.$store.state.form }}</pre>
  </div>
</template>

<script>
export default {
  name: 'app',
  methods: {
    submitForm() {}
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
