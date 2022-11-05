

/* 结构 */


/* 单文件组件   结构    交互  样式 */

/* template 不参与结构编译   执行里面的代码 */


<template>

<div class="demo">


    <h2>学校名称：{{schoolName}}</h2>
    <h2>学校地址：{{schoolAdd}}</h2>


    <button @click='show'>点我</button>
</div>


</template>


<script>


export default {
    //name:组件名   最好和文件名保持一致  
    name:'SchoolNa',
    data() {
        
        return {
            schoolName:'汇发云',
            schoolAdd:'上海'
        }
    },

    methods: {
        show() {
            alert(this.schoolName)
        }
    }
}

</script>





<style>



.demo {
    background-color: aqua;




}

</style>

