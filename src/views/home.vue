<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <div>Home</div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import axios from '../utils/axios'

export default defineComponent({
  setup () {
    axios
      .get('/users/XPoet')
      .then((res) => {
        console.log('res: ', res)
      })
      .catch((err) => {
        console.log('err: ', err)
      })
  }
})
</script>
<style lang="scss" scoped></style>
