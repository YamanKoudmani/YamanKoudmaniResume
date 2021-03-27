<template>
  <div class="parentContainer">
    <div class="container">
      <h1>{{ msg }}</h1>
      <p>{{ bio }}</p>
    </div>
    <div class="container">
      <img src="https://raw.githubusercontent.com/YamanKoudmani/YamanKoudmani/master/src/assets/Yaman.jpg">
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String,
    bio: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  margin: 20px;
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
  color: #42b983;
}
</style>
