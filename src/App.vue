<template>
  <div id="app">
    <ul v-if="numbers.length> 0">
      <li v-for="number in numbers">{{number}}</li>
      </ul>
  <h1>Sign in</h1>
  <button @click="addNew()"> Or let's sign up</button>

  <input type="text" v-model="title">
  <input type="text" v-model="theme">

    <img alt="Vue logo" src="./assets/logo.png">
    
  



<button @click="iAmClicked()">Sign in</button>
</div>
</template>

<script>
export default {
        data() {
            return {numbers:[],title:"Name:",theme:"Password:"}
        },
        methods: {
            iAmClicked() {
                this.title = 'Clicked';
            },
            addNew(){
              this.theme = 'cos';
            }
        }
}
        

;
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Comic, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: blue;
  text-align: center;
  color: #2c3e59;
  margin-top: 120px;
}
</style>
