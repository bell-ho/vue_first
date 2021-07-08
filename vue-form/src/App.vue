<template>
  <!--//v-on:submit.prevent : 새로고침을 막음-->
  <form v-on:submit.prevent="submitForm">
    <div>
      <!-- label은 input을 바라보게됨-->
      <label for="username">id : </label>
      <input id="username" type="text" v-model="username">
    </div>
    <div>
      <label for="password">pw : </label>
      <input type="password" id="password" v-model="password">
    </div>
    <button type="submit">login</button>
  </form>
</template>
<script>
import axios from 'axios';

export default {
  name: 'app',
//data에 function을 넣는이유 : component단위로 만들때는 component간의 데이터가 공유되지않게 하기위해서
  data: function () {
    return {
      username: '',
      password: ''
    }
  }, methods: {
    submitForm: function () {
      // event.preventDefault(); //새로고침을 막음
      console.log(this.username, this.password);
      const url = 'https://jsonplaceholder.typicode.com/users';
      const data = {
        username: this.username,
        password: this.password
      }
      axios.post(url, data).then(function (response) {
        console.log(response.data);
      }).catch(function (error) {
        console.log(error);
      });
    }
  }
}
</script>
<style>

</style>
