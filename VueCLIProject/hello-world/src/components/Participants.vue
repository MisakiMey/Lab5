<template>
  <div id="Participants">
  <div class="nameCheck">
            <ul>
                <li v-for="(name,index) in names" :key="index">
                    <label>
                        <input type="checkbox" :value="name" v-model="checknames"/>
                        <label>{{name}}</label>
                    </label>

                </li>
            </ul>
            <span>Checked Names:{{checknames}}</span>

        </div>
  </div>
</template>

<script>

export default {
  name: 'Participants',
  data(){
      return{
          names:["Karina","Ira","I =)", "Kira", "Anna"],
          checknames:[],
      }
  }
}
</script>

<style>
.nameCheck li{
    text-align: left;
    list-style-type: none;
}
</style>