<template>
    <div>
            <h1>Button Click in Vue</h1>
            <h2 v-html="myhtml"></h2>
            <h2 v-once>{{name}}</h2>
            <h2>{{name}}</h2>
            <h3>{{ok ? "yes" : "No"}}</h3>
            <button v-on:click="chngName">Change Name </button>
            <button v-bind:disabled="disableBtn" on:click="toggle">Change Status </button>
        </div>
</template>

<script>
export default {
    name : 'ButtonClick',

    data(){

        return{
            name : "Arif",
            ok:true,
            myhtml:"<h2>Call Html In VUE </h2>",
            disableBtn:true
        }
    },

    methods : {

        chngName(){

            this.name = "haifa"
        },

        toggle(){
            this.ok=!this.ok
        }

    }
}
</script>