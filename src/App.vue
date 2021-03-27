<template>
  <div id="app" class ="container">
    <HelloWorld msg="Yaman Koudmani" bio="Yaman Koudmani is a Computer Science student who loves tinkering with new technologies. He spends most of his time working on various computer projects, whether it is tinkering with new Operating Systems or repairing old computers, he finds joy in discovering new things in the realm of technology. This is just basic text as the website is still under construction used to test spacing. Thanks for visiting."/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
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
img {
  border-radius: 25%;
  width: 100%;
  height: auto;
  position: relative;               /* 2 */
  top: 50%;                         /* 3 */
  transform: translate(0, -50%)    /* 4 */
}
.parentContainer {
  display: flex;
}
.container {
  max-width: 1000px;
  margin: 30px auto;
  overflow: auto;
  min-height: 200px;
  min-width: 100px;
  /* border: 1px solid steelblue; */
  padding: 30px;
}
.btn {
  display: inline-block;
  background: #000;
  color: #fff;
  border: none;
  padding: 10px 20px;
  margin: 5px;
  border-radius: 5px;
  cursor: pointer;
  text-decoration: none;
  font-size: 15px;
  font-family: inherit;
}
.btn:focus {
  outline: none;
}
.btn:active {
  transform: scale(0.98);
}
.btn-block {
  display: block;
  width: 100%;
}
</style>
