<template>
  <div>
    <select v-model="city" name="" id="">
      <option value="02">서울</option>
      <option value="21">부산</option>
      <option value="064">제주</option>
    </select>
  </div>
</template>

<script>
export default {
  name: '',
  components: {},
  data() {
    return {
      city: "064"
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