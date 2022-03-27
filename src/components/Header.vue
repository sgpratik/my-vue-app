<template>
  <div class="container">
    <h1>{{ msg }}</h1>
    <p>
      To check out mypy-fhir project
      <a href="https://mypy-fhir.herokuapp.com/swagger" target="_blank">click here</a>.
    </p>
    <p> </p>
    <h4>To generate a random quote, please click the below button.</h4>
    <Quote />
  </div>
</template>

<script>
import Navbar from './Navbar.vue'
import Quote from './Quote.vue'

export default {
  name: 'Header',
  props: {
    msg: String
  },
  components: {
    Quote,
    Navbar
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.container {
  max-width: 500px;
  margin: 30px auto;
  overflow: auto;
  min-height: 300px;
  border: 1px solid rgb(209, 76, 15);
  padding: 30px;
  border-radius: 5px;
}

h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #d34e25;
}
</style>
