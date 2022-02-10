<template>
  <div id="app">
    <div id="nav">
      
      <button id="mainicons" type="button" class="btn btn-light " @click="homebutton()">Home</button> 
      <button id="mainicons" type="button" class="btn btn-light" @click="AboutButton()">About Us</button> 
      <button id="mainicons" type="button" class="btn btn-light" @click="ContactUsButton()">Contact</button>     
    
    </div>
    <router-view/>
  </div>
</template>
<script>
export default {
  data(){
    return
  },
  methods:{
    homebutton(){
      this.$router.push('/')
    },
    AboutButton(){
      this.$router.push('/about')
    },
    ContactUsButton(){
      this.$router.push('/contact')
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
  background: #edd2cb;
}

#nav {
  padding: 15px;
  background-color: #f55951;
}

#mainicons{
  margin-left: 5px;
  
  }
#authicons{
  float: right;
  margin-left: 5px;
}


#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
