<template>
  <div class="home">
    <HelloWorld greeting="Hello I am" name= "Aman Baid" />
    <div id="exp">
    <experience/>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import experience from '@/components/experience.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld,
    experience
  }
}
</script>
<style scoped>

</style>
