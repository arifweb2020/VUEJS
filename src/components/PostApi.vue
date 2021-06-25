<template>
    <div>
        <h1>Post Data through Api</h1>

        <form @submit="submitData" method="post">

 <input type="text"  v-model="post.title" placeholder="enter title" /><br>
        <input type="text"  v-model="post.body" placeholder="enter message"/>
       <br> <button v-on:click="submit">Send</button>
           </form>
        </div>
</template>

<script>
// import Vue from 'vue'
// import axios from 'axios'
// import VueAxios from 'vue-axios'
// Vue.use(VueAxios, axios)
export default {
    name : 'PostApi',
    
    
     data(){

        return{
            post: 
            {
                
                title:null,
                body:null
            }
        }
    },

    methods:{
        submitData(e){
            e.preventDefault();
            this.axios.post('https://jsonplaceholder.typicode.com/posts', this.post).then((res)=>{
                console.log(res)
            })
        }

    }
}
</script>