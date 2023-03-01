<template>
  <div id="app">
    <jsx-msg msg="Welcome to Your Vue.js App"/>
    <el-date-picker
      v-model="value1"
      type="yearrange"
      range-separator="至"
      start-placeholder="开始年份"
      end-placeholder="结束年份"
    />
  </div>
</template>

<script>
import jsxMsg from '@/components/jsxMsg.vue'

export default {
  name: 'App',
  components: {
    jsxMsg
  },
  data() {
    return {
      value1: ''
    }
  }
}
</script>

<style>
</style>
