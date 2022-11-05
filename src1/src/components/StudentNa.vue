<template>


<div id="id">
    <h2>学生名字：{{name}}</h2>
    <h2>学生年龄：{{age}}</h2>
    <button @click='show2'></button>
</div>
    
</template>


<script>

export default {
    //name:组件名   最好和文件名保持一致  MyName 
    name:'StudentNa',
    data() {
        
        return {
            name:'吴英',
            age:20
        }
    },

    methods: {
        show2() {
            alert('this.name')
        }
    }
}


</script>



<style>

</style>