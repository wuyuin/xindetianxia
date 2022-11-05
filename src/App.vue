<template>
<div>
  <SchoolXx></SchoolXx>
  <!-- <StudentXx   ref='stu'></StudentXx> -->
<!-- ref   相当于id  -->
<!-- ref 属性用来给元素/标签   h1     或者给子组件StudentXx 注册引用信息 （id替代者） -->
<!-- 获取：this.$refs.tiltle -->
  <!-- <h1 v-text='msg' ref='tiltle'></h1> -->
  <!-- :   v-bind:   动态单向绑定  把‘’ 内当成了表达式-->
<StudentXx name='linyu' :age='12'></StudentXx>
<hr/>

<!-- <StudentXx name='hahah' :age='45'></StudentXx> -->
<hr/>
<!-- <StudentXx name='kuku' ></StudentXx> -->

  <!-- <button @click='show2' ></button> -->
</div>
  
</template>

<script>

import SchoolXx from './components/SchoolXx.vue'
import StudentXx from './components/StudentXx.vue'
export default {
  name:'App',
  components: {
    SchoolXx,
    StudentXx,
  },

  // data() {
  //   return {
  //      msg:'我爱你 汇发'

  //   }
   

  // },
  // methods: {
  //   show2() {
  //     console.log(this.$refs.stu)
  //   }
  // }

}
</script>

<style>

</style>