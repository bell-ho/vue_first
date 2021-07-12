<template>
  <div>
<!-- v-model 은 내부적으로 value 의 속성을 사용하게됨-->
    <input type="text" v-model="valueModel"> |
    <input type="number" v-model.number="numberModel">
  </div>
</template>

<script>
export default {
  name: '',
  components: {},
  data() {
    return {
      valueModel: '한국',
      numberModel: 3
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