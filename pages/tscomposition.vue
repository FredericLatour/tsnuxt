<template>
  <div class="msg">
    <h2>TS Composition API</h2>
    <div>Message: {{ message }}</div>
    <div>Message2: {{ message2 }}</div>
    <div>Autre Message: {{ anotherMsg }}</div>
  </div>
</template>

<script lang="ts">
import { createComponent, reactive } from '@vue/composition-api'

export default createComponent({
  setup () {
    const message = reactive('coucou')
    const message2 = 'coucou2'
    return {
      message,
      message2
    }
  },
  asyncData () {
    return { anotherMsg: 'From asyncData' }
  }
})

</script>
