<template>
  <div id="app">
    
  <b-container fluid min-height="800px" class="bv-example-row">
  <b-row align="left">
    <b-col cols="6"><b-form-input placeholder="Enter your name"></b-form-input></b-col>
    <b-col><b-button>Search</b-button></b-col>
    <b-col><span>this is a test</span></b-col>
    <b-col><b-button>Add Entry</b-button></b-col>
  </b-row>
  

  <b-row><b-col><p>T</p></b-col></b-row>

  <b-row class="testing-greg">
    <b-col cols="4" >
    <b-list-group>
  <b-list-group-item>Cras justo odio</b-list-group-item>
  <b-list-group-item>Dapibus ac facilisis in</b-list-group-item>
  <b-list-group-item>Morbi leo risus</b-list-group-item>
  <b-list-group-item>Porta ac consectetur ac</b-list-group-item>
  <b-list-group-item>Vestibulum at eros</b-list-group-item>
  <b-list-group-item>Cras justo odio</b-list-group-item>
  <b-list-group-item>Dapibus ac facilisis in</b-list-group-item>
  <b-list-group-item>Morbi leo risus</b-list-group-item>
  <b-list-group-item>Porta ac consectetur ac</b-list-group-item>
  <b-list-group-item>Vestibulum at eros</b-list-group-item>
  <b-list-group-item>Cras justo odio</b-list-group-item>
  <b-list-group-item>Dapibus ac facilisis in</b-list-group-item>
  <b-list-group-item>Morbi leo risus</b-list-group-item>
  <b-list-group-item>Porta ac consectetur ac</b-list-group-item>
  <b-list-group-item>Vestibulum at eros</b-list-group-item>
  <b-list-group-item>Cras justo odio</b-list-group-item>
  <b-list-group-item>Dapibus ac facilisis in</b-list-group-item>
  <b-list-group-item>Morbi leo risus</b-list-group-item>
  <b-list-group-item>Porta ac consectetur ac</b-list-group-item>
  <b-list-group-item>Vestibulum at eros</b-list-group-item>
</b-list-group>
    </b-col>
    <b-col cols="8"><button v-on:click="getData">My Button</button></b-col>
    
  </b-row>
</b-container>
    <!-- <img alt="Vue logo" src="./assets/logo.png -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  </div>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'

const axios = require('axios');
      //require('promise/polyfill-done');

function main() {
   axios.get('http://localhost:3000/').then((response) => {
    console.log(response.data);
    return response;
  });
}


export default {
  name: 'App',
  components: {
    //HelloWorld
  },
  methods: {
    getData () {
      
      main();
 
  
   
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
div.testing-greg {
   height: 400px;
}
</style>
