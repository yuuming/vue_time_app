<template>
  <div id="app">
    <h1 class="happyMessage" v-if="['lucky person', 'happy person', 'funny person'].includes(who_i_am)">You have a glitter life!!! :)</h1>
    <label for="person_textbox">I am a </label><input type="textbox" id="person_textbox" placeholder= "what person type you are" v-model="who_i_am"><br>
    <b v-if="!['lucky person', 'happy person', 'funny person'].includes(who_i_am)">Please be happy and smile more!</b>
    <div v-if="who_i_am != 'minimalist'">
       <h2>Welcome to VuePractice page!</h2>
    <h3 id="app">Vue is very interesting</h3>

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