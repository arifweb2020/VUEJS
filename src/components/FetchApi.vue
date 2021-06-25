<template>
    <div>
        <h1>Api Fetch in Vue </h1>
        <h2 v-for="item in list" :key="item.id">{{item.name}}</h2>
        </div>
</template>

<script>
export default {
    name : 'FetchApi',

    data(){

       return{
           list:[]
       }
    },

    mounted(){

        fetch("https://thefacevalue.in/api/index.php").then((res)=>{
            return res.json()
        }).then((res1)=>{
            const res2 = res1.data
            this.list=res2
            console.log(res2)
        })
    }
}



</script>