<template>
  <header>
    <h1>{{ dataprops }}</h1>
    <button v-on:click="sendEvent">send</button>
  </header>
</template>
<script>
export default {
  props: ['dataprops'],
  methods: {
    sendEvent: function () {
      this.$emit('renew');  //renew 이벤트 방출
    }
  }
}
</script>
<style>

</style>
