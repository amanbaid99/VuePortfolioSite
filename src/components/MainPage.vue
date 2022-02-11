<template>
<div  id="parent" class="d-inline-flex p-2">
  <div id = "image">
    <img src="../assets/profile.png" alt="no image">
  </div>
  <div class="hello">
      <h5>Web Developer</h5>
      <p id="name">{{name}}</p>
      <button id="Buttons" type="button" class="btn btn-dark">Download CV</button> &nbsp;
      <button id="Buttons" type="button" class="btn btn-dark" @click="AboutButton()">About</button><br>
      <img src="https://img.icons8.com/ios-glyphs/45/000000/github.png"/>
      <img src="https://img.icons8.com/ios-filled/45/000000/gmail-new.png"/>
      <img src="https://img.icons8.com/ios-filled/45/000000/apple-phone.png"/>
      <img src="https://img.icons8.com/material/45/000000/instagram-new--v1.png"/>
  </div>
</div>
</template>

<script>
export default {
  name: 'MainPage',
  props: {
    name: String,
    greeting: String,
  },
methods:{
    homebutton(){
      this.$router.push('/')
    },
    AboutButton(){
      this.$router.push('/about')
    },
  }
}
</script>

<style scoped>

.hello{  
  font-family:'Anton', sans-serif; 
  padding: 30px;
  float: right;
}
#parent{
  background: #edd2cb;
  
}

img{
  padding: 40px;
  border-radius: 50%;
}
  #name{
    font-size: 100px;
  }
  #Buttons{
    border-radius: 10px;
    }
a {
  color: #42b983;
}


</style>
