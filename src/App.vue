<template>
<div>
  <!-- <SchoolXx></SchoolXx> -->
  <!-- <StudentXx   ref='stu'></StudentXx> -->
<!-- ref   相当于id  -->
<!-- ref 属性用来给元素/标签   h1     或者给子组件StudentXx 注册引用信息 （id替代者） -->
<!-- 获取：this.$refs.tiltle -->
  <!-- <h1 v-text='msg' ref='tiltle'></h1> -->
  <!-- :   v-bind:   动态单向绑定  把‘’ 内当成了表达式-->
<!-- <StudentXx name='linyu' :age='12'></StudentXx> -->
<hr/>

<!-- <StudentXx name='hahah' :age='45'></StudentXx> -->
<hr/>
<!-- <StudentXx name='kuku' ></StudentXx> -->

  <!-- <button @click='show2' ></button> -->
  <!-- vue 脚手架的组件标签在使用时可以写成双标签 <h></h>  也可以写成  <StudentAa/>自闭和标签的形式  注意写成自闭和标签时 /放在后面  组件的名字采用StuentAa写法  -->

  <StudentAa/>
  <SchoolAa/>

</div>
  
</template>

<script>
import SchoolAa from './components/SchoolAa.vue'
import StudentAa from './components/StudentAa.vue'
// import SchoolXx from './components/SchoolXx.vue'
// import StudentXx from './components/StudentXx.vue'
export default {
  name:'App',
  components: {
    // SchoolXx,
    // StudentXx,
    SchoolAa,
    StudentAa,
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