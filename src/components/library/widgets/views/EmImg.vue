<!--
 * @Description:
 * @Author: 吴文周
 * @Github: https://github.com/fodelf
 * @Date: 2019-05-08 12:31:07
 * @LastEditors: 吴文周
 * @LastEditTime: 2019-08-23 08:45:53
 -->
<template>
  <div ref="widget"
       class="widget"
       v-bind:style="{ height: height, width: width,top:top,left:left,padding:padding}">
    <img :src="src"
         class="img"
         draggable="false" />
    <!-- <div v-show="!ishow">
      <div></div>
      <div></div>
    </div> -->
  </div>
</template>
<script>
import viewVue from './view.vue'
export default {
  name: 'Img',
  extends: viewVue,
  data () {
    return {
      widgetName: 'EmImg',
      src: ''
    }
  },
  methods: {
    setSrc (src) {
      this.src = src
    },
    getSrc () {
      return this.src
    }
  }
}
</script>

<style   lang="scss" scoped>
.img {
  height: 100%;
  width: 100%;
}
</style>
