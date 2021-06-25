<template>
    <div>
        <!-- <input type="text"  v-model="loginForm.username" placeholder="enter name" /><br>
        <input type="password"  v-model="loginForm.password" placeholder="enter password"/>
       <br> <button v-on:click="submit">Login</button> -->
<p >
    <b>correct the following errors</b>
    <ul>
        <li v-for="e in loginForm.error" v-bind:key="e.id">
            {{e}}
            </li>
        </ul>


    </p>

       <form @submit="login">

 <input type="text"  v-model="loginForm.username" placeholder="enter name" /><br>
        <input type="password"  v-model="loginForm.password" placeholder="enter password"/>
       <br> <button v-on:click="submit">Login</button>
           </form>
        
        </div>
</template>

<script>
export default {
    name:'Form',

    // methods: {
    //     submit(){
    //         console.log("login data", this.loginForm.username , this.loginForm.password)

    //     }
    // }
     methods: {
         login(e)
        {
            this.loginForm.error=[];
            if(this.loginForm.username && this.loginForm.password){
                console.log("no error")
            }
            if(!this.loginForm.username){
                this.error.push("username is required")
            }
            if(!this.loginForm.password){
                this.error.push("password is required")
            }
            console.log("login data", this.loginForm.username , this.loginForm.password)
            e.preventDefault();

        }
    },

    data(){

        return{
            loginForm: 
            {
                error:null,
                username:null,
                password:null
            }
        }
    }

}
</script>>