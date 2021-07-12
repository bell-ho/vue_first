<template>
  <div>
    <label for="">
      <input type="checkbox" v-model="checked">{{checked}}
      <input type="checkbox" v-model="checked2" true-value="yes" false-value="no">{{checked2}}
    </label>
  </div>

  <div>
    <label for=""><input type="checkbox" value="서울" v-model="checked3">서울</label>
    <label for=""><input type="checkbox" value="부산" v-model="checked3">부산</label>
    <label for=""><input type="checkbox" value="제주" v-model="checked3">제주</label>
  </div>
  <br>
  <span>체크한 지역:{{checked3}}</span>
</template>

<script>
export default {
  name: '',
  components: {},
  data() {
    return {
      checked: true,
      checked2: true,
      checked3: []
    };
  },
  setup() {

  },
  created() {

  },
  mounted() {

  },
  unmounted() {

  },
  methods: {}
}
</script>

<style scoped>

</style>