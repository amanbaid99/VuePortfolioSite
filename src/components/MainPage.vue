<template>
<div  id="parent" class="d-inline-flex p-2">
  <div id = "image">
    <img src="../assets/profile.png" alt="no image">
  </div>
  <div class="hello">
      <h5>Web Developer</h5>
      <p id="name">{{name}}</p>
      <button id="Buttons" type="button" class="btn btn-dark" @click="ResumeButton()">Check Resume</button> &nbsp;
      <button id="Buttons" type="button" class="btn btn-dark" @click="AboutButton()">About</button><br>
      <img id="icons" src="https://img.icons8.com/ios-glyphs/45/000000/github.png" @click="github()"/>
      <img id="icons" src="https://img.icons8.com/ios-filled/45/000000/linkedin.png"/>
      <img id="icons" src="https://img.icons8.com/ios-filled/45/000000/gmail-new.png"/>
      <img id="icons" src="https://img.icons8.com/material/45/000000/instagram-new--v1.png"/>
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
    ResumeButton(){
      window.open('https://drive.google.com/file/d/1i-XpoDyE8MnE93Xi5CkR5jsp6BoBGnUf/view')
    },
    github(){
      window.open('https://github.com/amanbaid99')
    }

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
  #name:hover{
    color: orangered;
  }
  #Buttons{
    border-radius: 10px;
    }
  #Buttons:hover{
    color:blue;
  }
  #icons:hover{
    transform:scale(1.25)
  }
a {
  color: #42b983;
}


</style>
