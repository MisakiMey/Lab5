<template>
  <div id="userdata">
<input placeholder = "Name" v-model = "name"/>
<input placeholder = "Surname" v-model = "surname"/>
<input placeholder = "Age" v-model = "age"/>
<input placeholder = "City" v-model = "city"/>
<h2>Поточні дані користувача</h2>
        <div  class="conf">
    <table>
        <tr>
            <td>Name</td>
            <td>Surname</td>
            <td>Age</td>
            <td>City</td>
        </tr>
        <tr>
            <td>{{name}}</td>
            <td>{{surname}}</td>
            <td>{{age}}</td>
            <td>{{city}}</td>
        </tr>
    </table>
    </div>
</div>
</template>

<script>

export default {
  name: 'userdata',
  data(){
return{
    name:"",
    surname:"",
    age: null,
    city:"",
    }
    }
}
</script>

<style>

</style>