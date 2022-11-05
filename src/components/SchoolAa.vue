<template>
  <div>
    <h2 @click='show2'>Aa学校地址:{{address}}</h2>
    <h2>Aa 学校名称:{{Sname}}</h2>
  </div>
</template>

<script>
export default {
    name: 'SchoolAa',
    data() {
        return {
            address: '石家庄',
            Sname:'铁道学院'
        }
    },
    methods: {
        show2() {
            alert(this.address)

        }
    }

}
</script>

<style>
div {
    background-color: bisque;
}

</style>