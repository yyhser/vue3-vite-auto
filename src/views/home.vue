<template>
  <div class="text">123</div>
</template>
<script lang="ts">
import { defineComponent } from 'vue'
import axios from '../untils/axios'
export default defineComponent({
  setup() {
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
<style lang="less">
.text {
  color: #f00;
}
</style>
