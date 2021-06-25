<template>
    <div>
        <input type="text"  v-model="loginForm.username" placeholder="enter name" /><br>
        <input type="password"  v-model="loginForm.password" placeholder="enter password"/>
       <br> <button v-on:click="submit">Login</button>
        
        </div>
</template>

<script>
export default {
    name:'Form',

    methods: {
        submit(){
            console.log("login data", this.loginForm.username , this.loginForm.password)

        }
    },

    data(){

        return{
            loginForm: 
            {
                username:null,
                password:null
            }
        }
    }

}
</script>>