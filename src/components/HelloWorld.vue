<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<style scoped>
.hello {
  margin-top: 20px;
}

h1 {
  font-size: 2.5em;
  color: #42b983;
}
</style>
