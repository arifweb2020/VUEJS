<template>
    <div>
        <h1>For Loop </h1>
        <table>
            <tr>
                <th>id</th>
                <th>Name</th>
                <th>email</th>
                </tr>

                <tr v-for="data in users" :key="data.id">
                <td>{{data.id}}</td>
                <td>{{data.name}}</td>
                <td>{{data.email}}</td>
                    </tr>
        </table>
        </div>
</template>

<script>
export default {
    name : 'ForLoop',
    data(){

        return {
            users: [

                {id:1,name:'peter',email:'arif@gmail.com'},
                {id:2,name:'john',email:'john@gmail.com'},
                {id:3,name:'lela',email:'lela@gmail.com'},
            ]
        }
    }
}
</script>

<style  scoped>

table,tr,th,td{
    border: 2px solid black;
    border-collapse: collapse;
    padding: 20px;
}

</style>