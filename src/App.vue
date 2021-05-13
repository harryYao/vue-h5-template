<template>
  <div id="app">
    <router-view />
  </div>
</template>
<script>
import { removeWatermark, setWaterMark } from '@/utils/watermark'

export default {
  name: 'App',
  mounted() {
    setWaterMark('张三', '123456789')
  },
  destroyed() {
    removeWatermark()
  }
}
</script>
<style lang="scss"></style>
