<template>
  <div id="app">
    <img width="100" alt="Vue logo" src="./assets/logo.png">
    <form :action="formUrl" method="post">
      <input required name="email" placeholder="Email" type="text">
      <input required name="fullName" placeholder="Full name" type="text">
      <textarea required name="message" placeholder="Your message" id="" cols="30" rows="10"></textarea>
      <button type="submit">Submit</button>
    </form>
  </div>
</template>

<script>

export default {
  name: 'App',
  computed: {
    formUrl() {
      return 'https://fabform.io/f/9DrEaKE'
    }
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
  display: flex;
  align-items: center;
  flex-direction: column;
}
form {
  display: flex;
  flex-direction: column;
  width: 300px;
}
input, textarea {
  padding: 10px;
  margin-top: 10px;
}
button {
  margin-top: 10px;
  padding: 10px;
}
</style>
