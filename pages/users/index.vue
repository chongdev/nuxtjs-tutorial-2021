<template>
<div>
    <table>
        <tr v-for="(user, index) in users" :key="index">
            <td>{{user.id}}</td>
            <td>{{user.name}}</td>
        </tr>
    </table>
 </div>
</template>

<script>
export default {
    data(){

        let users = [];
        users.push({id: 1, name: 'A'});
        users.push({id: 2, name: 'B'});

        return{
            users: users
        }
    }
}
</script>