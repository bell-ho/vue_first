<template>
  <div>
    <h1>Computed Full name : {{ fullName }}</h1>
    <h1>Watch Full name : {{ fullName2 }}</h1>
    <button type="button" @click="changeName">변경</button>
  </div>
</template>

<script>
export default {
  name: '',
  components: {},
  data() {
    return {
      firstName: 'J',
      lastName: 'H',

      firstName2: 'Lee',
      lastName2: '종호',

      fullName2: ''
    };
  },
  computed: {
    fullName() {  //fullName은 함수이자 동시에 Vue인스턴스의 데이터 키 값
      return this.firstName + ' ' + this.lastName;
    }
  },
  watch:{
    firstName2() {
      this.fullName2 = this.firstName2 + ' ' + this.lastName2;
    },
    lastName2() {
      this.fullName2 = this.firstName2 + ' ' + this.lastName2;
    }
  },
  setup() {

  },
  created() {

  },
  mounted() {

  },
  unmounted() {

  },
  methods: {
    changeName() {
      this.firstName2 = '이';
    }
  }
}
</script>

<style scoped>

</style>