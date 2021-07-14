<template>

  <div v-bind:style="styleObject">
    인라인 스타일 바인딩
  </div>
</template>

<script>
export default {
  name: '',
  components: {},
  data() {
    return {
      sampleData: ''
      , styleObject: {
        color: 'red'
        , fontsize: '13px'
      }
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