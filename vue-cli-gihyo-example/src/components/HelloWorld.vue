<template>
  <div id="app">
    <h1>{{ msg }}</h1>
    <input type="checkbox" id="my_checkbox" v-model="checked">
    <label for="my_checkbox">Check box.</label>
  </div>
</template>

<style>
.message { color: #a647dd; }
</style>

<script>
export default {
  name: 'app',
  data () {
    return {
      msg: 'Vue Practice Page!!!!',
      checked: false
    }
  },
  watch: {
    checked: function (val) {
      if (val) {
        this.msg = 'Second message!'
      }
      else {
        this.msg = 'First message!'
      }
    }
  }
}
</script>