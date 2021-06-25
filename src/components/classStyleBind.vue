<template>
    <div>
        <h1 class="main-heading">class Style Bind</h1>
        <h2 v-bind:style="{color:'green'}"> style bind </h2>
        <!-- <h2 v-bind:class="{myBg:true}"> class binding with object </h2> -->

        <h2 v-bind:class="{myBg:show,mycolor:show}"> class binding with object </h2>
        </div>
</template>

<script>
export default {
    name : 'classStyleBind',
    data(){
        return{
            show:true
        }
    }

}
</script>

<style scoped>
.main-heading{
    color:purple
}
.myBg{
    background: grey;
}
.mycolor{
    color:red;
}
</style>