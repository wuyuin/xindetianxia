<template>

<div>



  <img src="./assets/logo.png" alt="logo">
<SchoolNa></SchoolNa>
<StudentNa></StudentNa>




</div>

  
</template>

<script>


import SchoolNa from './components/SchoolNa.vue'
import  StudentNa from './components/StudentNa.vue'

export default {
    name:'App',
  components: {
    SchoolNa,
    StudentNa,
   
  }
}
</script>

<style>

</style>