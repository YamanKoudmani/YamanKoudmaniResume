<template>
  <div id="app" class="globalContainer">
    <HelloWorld msg="Yaman Koudmani"  bio= "Hello, and welcome to my site. <br> <br> If you are here to learn more about me, you've come to the right place.
    I'm a Computer Science student who loves tinkering with new technologies. That means I spend most of my time working on various computer projects, whether it is tinkering with new Operating Systems or repairing old computers. I find joy in learning new things in the realm of technology. 
    <br> <br> Below you will find my general Resume. <br> Thanks for visiting."/>
      <Button @toggle-resume="toggleResF" text="View Resume:" />
      <div class="container" v-show="showRes">
        <PDFViewer />
      </div>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Button from './components/Button.vue'
import PDFViewer from './components/PDFViewer.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    Button,
    PDFViewer
  },
  data() {
    return {
      showRes: false
    }
  },
  methods: {
    toggleResF(){
      this.showRes = !this.showRes
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
}
img {
  border-radius: 25%;
  width: 100%;
  max-width: 200px;
  height: auto;
  position: relative;               /* 2 */
  top: 50%;                         /* 3 */
  transform: translate(0, -50%)    /* 4 */
}
.globalContainer{
  border: 2px solid black;
  margin: 5px;
  background:rgba(216, 216, 216, 0.61)

}
.parentContainer {
  display: flex;
  width: 100%;
  /*border: 1px solid red; */
  margin: 0 auto;

}
.container {
  margin: 0 auto;
  overflow: auto;
  min-height: 200px;
  min-width: 150px;
  padding: 30px;
  /* border: 1px solid steelblue; */
}
.btn {
  display: block;
  background: #000;
  color: #fff;
  border: none;
  padding: 10px 20px;
  margin: 20px;
  border-radius: 5px;
  cursor: pointer;
  text-decoration: none;
  font-size: 30px;
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
