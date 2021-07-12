<template>
  <h1>{{htmlString}}</h1>
  <div v-html="htmlString"></div>
</template>

<script>
export default {
  name: '',
  components: {},
  data() {
    return {
      htmlString: '<p style="color: red;">This is a red String</p>',
      // htmlString: 'gg'
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