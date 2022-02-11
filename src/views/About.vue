<template>
  <div class="about">
    <h1>This is an about page</h1>
    <button id="Buttons" type="button" class="btn btn-dark" @click="homebutton()">Home</button><br>
  </div>
</template>

<script>
export default {
  data() {
    return
    
  },
  methods:{
   homebutton(){
      this.$router.push('/')
    }
  }
}
</script>
