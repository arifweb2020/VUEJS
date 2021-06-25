<template>
    <div>
        <h1>Data Binding</h1>
        <input type="text" v-model="msg">
        <h2>{{msg}}</h2>
        </div>
</template>

<script>
export default {
    name : 'DataBinding',
    data(){

        return {

            msg:'hello'
        }
    }
}
</script>