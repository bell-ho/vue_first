<template>
  <div class="container" v-bind:class="{
      'active':isActive, 'text-red':hasError }">
    Class Binding
  </div>
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
      isActive: true,
      hasError: false,
      styleObject: {
        color: 'red',
        fontsize: '13px'
      },
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
container {
  width: 100%;
  height: 200px;
}

.active {
  background-color: yellow;
  font-weight: bold;
}

.text-red {
  color: red;
}

</style>