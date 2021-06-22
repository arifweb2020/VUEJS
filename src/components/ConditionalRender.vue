<template>
    <div>
        <h1 v-if="show"> conditional render | if condition</h1>
        <h1 v-else>Other wise this will show</h1>
        </div>
</template>

<script>
export default {
    name: 'ConditionalRender',
    data(){
        return{show:true}
    }
}
</script>>