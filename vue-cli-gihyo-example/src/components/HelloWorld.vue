<template>
  <div id="app">
    <h1 v-if="['lucky person', 'happy person', 'funny person'].includes(who_i_am)">You have a glitter life!!! :)</h1>
    <label for="person_textbox">I am a </label><input type="textbox" id="person_textbox" placeholder= "lucky person , happy person, funny person" v-model="who_i_am"><br>
    <b v-if="!['person', 'cool person', 'minimalist'].includes(who_i_am)">You must be a lucky person, happy person, or funny person.</b>
    <div v-if="who_i_am != 'minimalist'">
       <h2>Welcome to VuePractice page!</h2>
    <h3>Vue is very interesting</h3>

    </div>
  </div>
</template>
 
<script>
export default {
  name: 'app',
  data () {
    return {
      who_i_am: 'human'
    }
  },
  watch: {
  }
}
</script>