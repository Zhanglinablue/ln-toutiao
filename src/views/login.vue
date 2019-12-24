<template>
  <div id="conent-login">
<el-card class="box-card">
  <img src="../assets/logo_index.png" >
<el-form ref='form'>
  <el-form-item>
    <el-input v-model="form.code" placeholder="请输入手机号"></el-input>
  </el-form-item>
   <el-form-item>
    <el-input v-model="form.number" placeholder="请输入验证码" style="width:264px;margin-right:10px"></el-input>
   <el-button>验证码</el-button>
     <el-checkbox :value="true" style="margin-top:20px">我已阅读并同意签订条约</el-checkbox>
      <el-button type="primary" style="width:100% ;margin-top:30px">登录</el-button>
  </el-form-item>
</el-form>
</el-card>
  </div>
</template>

<script>
export default {
  data () {
    return {
      form: {
        code: '',
        number: ''

      }
    }
  }
}
</script>

<style lang="less" scoped>
#conent-login{
  width: 100%;
  height: 100%;
  position: absolute;
  left: 0;
  top: 0;
  background: url('../assets/login_bg.jpg') no-repeat center/cover;
  .box-card{
    position: absolute;
    left: 50%;
    top: 50%;
    transform: translate(-50%,-50%);
    width: 400px;
    height: 360px;
    img{
      display: block;
      margin: 0 auto;
      width: 180px;
      margin-bottom: 20px;
    }
  }
}
</style>
