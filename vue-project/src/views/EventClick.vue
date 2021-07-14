<template>
  <div>
    <button type="button" @click="increaseCounter">Add 1</button>
    <button type="button" @click="setCounter(0)">Set 0</button>
    <button type="button" @click="one() , two()">click</button>
    <p>The counter is : {{ counter }}</p>
  </div>
</template>

<script>
export default {
  name: '',
  components: {},
  data() {
    return {
      sampleData: ''
      , counter: 0
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
    increaseCounter() {
      this.counter = this.counter + 1;
    }
    , setCounter(v) {
      this.counter = v;
    }
    , one() {
      alert('One');
    }
    , two() {
      alert('Two');
    }
  }
}
</script>

<style scoped>

</style>