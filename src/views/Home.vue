<template>
  <div class="home">
    <MainPage greeting="Hello I am" name= "Aman Baid" />
    <hr>
    <div>
    <experience/><hr>
    <academics/><hr>
    <awards/><hr>
    <hobbies/><hr>
    </div>
  </div>
</template>

<script>
import MainPage from '@/components/MainPage.vue'
import experience from '@/components/experience.vue'
import academics from '@/components/academics.vue'
import awards from '@/components/awards.vue'
import hobbies from '@/components/hobbies.vue'

export default {
  name: 'Home',
  components: {
    MainPage,
    experience,
    academics,
    awards,
    hobbies
  }
}
</script>
<style>

</style>
