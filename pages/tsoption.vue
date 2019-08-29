<template>
  <div class="msg">
    <h2>TS Classic Options API</h2>
    <div>Message: {{ message }}</div>
    <div>Autre Message: {{ anotherMsg }}</div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  data () {
    return {
      message: 'Coucou'
    }
  },
  asyncData () {
    return { anotherMsg: 'another message' }
  }

})
</script>
