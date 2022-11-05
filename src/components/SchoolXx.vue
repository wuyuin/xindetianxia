<template>
  <div>
    <h2>学校地址： {{address}}</h2>
    <h2> 学校名字：{{name}}</h2>
    <button @click="show1"></button>
  </div>
</template>

<script>
export default {
    name:'SchoolXx',
    data() {
        return {
            address:'河北',
            name:'谈固'
        }
       
    },
    methods: {
        show1() {
            alert(this.name)
        }
    }

}
</script>

<style>
div {
    background-color: brown;
}

</style>