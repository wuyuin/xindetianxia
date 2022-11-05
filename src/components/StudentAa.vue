<template>
  <div>


    <h2 @click='show'> Aa的名字：{{name}}</h2>
    <h2>Aa的性别：{{sex}}</h2>

  </div>
</template>

<script>
export default {
    name: 'StudentAa',
    data() {
        return {
            name:' Ajax',
            sex: '男'
        }
    },
    methods: {
        show() {
            alert(this.name)
        }

    }

}
</script>

<style>

div {
    background-color: coral;
}

</style>