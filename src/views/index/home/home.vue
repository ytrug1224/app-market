<!--
 * @Description:主页
 * @Author: 吴文周
 * @Github: https://github.com/fodelf
 * @Date: 2019-06-11 18:59:40
 * @LastEditors: 吴文周
 * @LastEditTime: 2019-08-27 22:42:54
 -->
<template>
  <div id="mainHome">
    <!-- <div class='logoNav clearfix'>
      <p class='logoTit'>
        <span>易推广</span>
      </p>
      <el-menu :default-active="activeIndex"
               class="el-menu-demo"
               mode="horizontal"
               @select="handleSelect">
        <el-menu-item index="1">产品特性</el-menu-item>
        <el-menu-item index="2">我的站点</el-menu-item>
        <el-menu-item index="3">数据统计</el-menu-item>
      </el-menu>
    </div> -->
    <div class='startCon clearfix'>
      <div class='leftDiv'>
        <span class='line1'></span>
        <p>十分钟完成<br />智能营销页搭建</p>
        <span class='line2'></span>
        <button class='startBtn'
                @click="startOnce()">立即开始</button>
      </div>
      <div class='rightDiv'>

      </div>
      <!-- <el-form :label-position="labelPosition"
               label-width="80px"
               :model="form">
        <el-form-item label="用户名">
          <el-input v-model="form.username"></el-input>
        </el-form-item>
        <el-form-item label="密码">
          <el-input v-model="form.password"></el-input>
        </el-form-item>
        <el-button @click="login"> 登陆</el-button>
        <el-form-item label="用户名">
          <el-input v-model="form.username1"></el-input>
        </el-form-item>
        <el-form-item label="密码">
          <el-input v-model="form.password1"></el-input>
        </el-form-item>
        <el-button @click="login"> 注册</el-button>
      </el-form> -->
    </div>
    <div class="footer">免责声明：当前项目为初级学习阶段与git开源仿照项目无异，有借用第三方的设计，为此申明免责。
      严肃告知：落地页中不得出现危害，社会道德与中国法律的文字与图片否则后果自负</div>
  </div>
</template>

<script>
// import { login, register } from '@/api/index/login.js'
// import { setToken } from '@/utils/auth'
// import md5 from 'js-md5'
export default {
  name: 'Main',
  data () {
    return {
      activeIndex: '1',
      form: {
        username: '',
        password: '',
        username1: '',
        password1: ''
      }
    }
  },
  components: {
  },
  created () {

  },
  mounted () {

  },
  methods: {
    // 立即开始
    startOnce () {
      this.$router.push({
        path: '/control'
      })
    }
    // handleSelect (key, keyPath) {
    //   if (key === 2) {
    //     this.$router.push({ path: '/control' })
    //   } else if (key === 3) {
    //     this.$router.push({ path: '/dashBoard' })
    //   }
    // },
    /**
     * @name: login
     * @description: 登陆方法
     * @param {type}: 默认参数
     * @return {type}: 默认类型
     */
    // login () {
    //   login(this.form).then((res) => {
    //     setToken(res.token)
    //     localStorage.setItem('userId', res.userId)
    //   }).catch(() => {

    //   })
    // },
    /**
     * @name: login
     * @description: 登陆方法
     * @param {type}: 默认参数
     * @return {type}: 默认类型
     */
    // register () {
    //   let param = {
    //     username: this.form.username1,
    //     password: md5(this.form.password1)
    //   }
    //   register(param).then((res) => {
    //     console.log('注册成功')
    //   }).catch(() => {

    //   })
    // }
  }
}
</script>

<style  lang="scss" scoped>
@import "./home.scss";
</style>
