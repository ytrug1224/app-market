<!--
 * @Description:
 * @Author: 吴文周
 * @Github: https://github.com/fodelf
 * @Date: 2019-08-12 22:23:09
 * @LastEditors: 吴文周
 * @LastEditTime: 2019-08-23 08:21:02
 -->
<template>
  <div id="app">
    <mainArea></mainArea>
  </div>
</template>
<script>
import mainArea from '@/views/preview/mainArea/mainArea.vue'
export default {
  name: 'app',
  components: {
    mainArea
  }
}
</script>

<style lang="scss">
@import "../../assets/css/base.css";
.widget {
  font-size: 14px;
}
</style>
