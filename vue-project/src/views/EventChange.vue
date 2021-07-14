<template>
  <div>
    <select name="" id="" v-model="selectedValue" @change="changeSelect">
      <option value="서울">서울</option>
      <option value="부산">부산</option>
      <option value="제주">제주</option>
    </select>
  </div>
</template>

<script>
export default {
  name: '',
  components: {},
  data() {
    return {
      sampleData: ''
      , selectedValue: '서울'
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
  methods: {
    changeSelect() {
      alert(this.selectedValue);
    }
  }
}
</script>

<style scoped>

</style>