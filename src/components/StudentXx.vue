// template 最终不会解析  

<template>
  <div>
    <h1> 学生信息 {{msg}}</h1>

<h2>学生名字：{{name}}</h2>
<h2>学生年龄：{{Myage}}</h2>
<button @click='show'></button>


  </div>
</template>

<script>
// 组件VueComponent 实例vc 和vm几乎一样  所以用法几乎一样  除了 组件不能定义el  操作容器只能是vm    并且组件的数据不能写对象式 必须写成函数式   
export default {

    name:'StudentXx',
    // 组件的data必须是函数式的  不能是对象式的
    data() {
        return {
            msg:'我是一个汇法人',
            Myage:this.age

            
        }

    },
    methods: {
        show() {
            //this 指的是VueComponent
            this.Myage++
           
        }

    },
    // props的三种方式    
    // props:['name','age']   简单接收   数组
    // props 的优先级比data() 数据里面高  vc 优先读取props 
    props:['name','age', 'phone']
    // 对象  接受的同时对数据进行限制   什么类型
    // props: {
    //     name: String,
    //     age: Number,
    // }

    // props: {
    //     name: {
    //         type:String,
    //         required:true
    //     },

    //     age: {
    //         type:Number,
    //         default:99
    //     }
    // }





    

}
</script>

<style>
div {
    background-color: blueviolet;
}
</style>