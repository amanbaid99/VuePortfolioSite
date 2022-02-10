<template>
<div  id="parent" class="d-inline-flex p-2">
  <div id = "image">
    <img src="../assets/profile.png" alt="no image">
  </div>
  <div class="hello">
      <h5>Web Developer</h5>
      <p id="name">{{name}}</p>
      <button id="CVButton" type="button" class="btn btn-dark">Download CV</button>
  </div>
</div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    name: String,
    greeting: String,

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
  #CVButton{
    border-radius: 10px;
    }
a {
  color: #42b983;
}


</style>
