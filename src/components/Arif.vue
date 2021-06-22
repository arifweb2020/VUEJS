<template>
<div>
    <h1>This is Arif component {{data}}</h1>
    <h2>i m working in {{cmp}}</h2>
    <button v-on:click="hello('arif')">Check</button>
    </div>
</template>


<script>
export default {
  name: 'Arif',
  props:{
      data:String,
      cmp:String
  },
  methods:{
      hello(arif){
          alert(`ind win ${arif}`)
      }
  }
  
}
</script>

<style  scoped>
h1{
    color: red;
}
</style>>