<template>
  <div id="comment">
  <label>
            <textarea v-model="message"></textarea>
        </label>
        <button @click="sad">Send</button>
        <div class="com">
            <ul>
                <li v-for="(mess,index) in comments" :key="index">
                    <div class="comments">
                        <strong>{{mess.message}}</strong>
                        <span>{{mess.time}}</span>
                    </div>
                </li>
            </ul>

        </div>
  </div>
</template>

<script>
export default {
  name: 'comment',
  data() {
      return{
          message:"",
          comments:[],
      }
  },
  methods:{
      sad (){
          let time=`${new Date().getHours()}:${new Date().getMinutes()}`;
          let mess = {
              message: this.message,
              time: time,
          }
          this.comments.push(mess)
      }
  } 
}
</script>

<style>
.com li{
        list-style-type: none;
        text-align: left;
    }
.comments span{
    margin-left: 10px;
}
</style>