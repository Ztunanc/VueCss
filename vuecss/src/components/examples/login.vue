<template>
  <div class="login">
      <div class="login-container">
          <div class="left-container">
              <div class="title">
                  <span>登录</span>
              </div>
              <div class="input-container">
                  <input type="text" name="username" placeholder="用户名">
                  <input type="text" name="password" placeholder="密码">
              </div>
              <div class="message-container">
                  <span>忘记密码</span>
              </div>
          </div>
          <div class="right-container">
              <div class="register-container">
                  <span class="register">注册</span>
              </div>
              <div class="action-container">
                  <span>提交</span>
              </div>
          </div>
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
*{
    margin: 0;
    padding: 0;
}
.login{
    height: 100%;
    width: 100%;
    position:fixed;
    background: linear-gradient(to bottom right,rgb(114,135,254),rgb(130,88,186));
    /* 设置文字不可选中 */
    -webkit-user-select:none;
     -moz-user-select:none;
     -ms-user-select:none;
     user-select:none;
}
.login-container{
    width: 600px;
    margin: 0 auto;
    margin-top: 10%;
    border-radius: 15px;
    box-shadow: 0 10px 50px 0 rgb(59, 45, 159);
    background-color: rgb(95, 76, 194);
}
.login-container .left-container{
    background-image: linear-gradient(to bottom right,rgb(118,76,163),rgb(97,103,211));
    display: inline-block;
    width:330px;
    height: 315px;
    border-top-left-radius: 15px;
    border-bottom-left-radius: 15px;
    padding: 60px;
}
.login-container .left-container .title{
    color: #fff;
    font-size: 18px;
    font-weight: 200;
}
.login-container .left-container .title span{
    border-bottom: 3px solid rgb(237,221,22);
}
.login-container .left-container .input-container{
    padding: 10px 0;
}
.login-container .left-container .input-container input{
    border: 0;
    background: none;
    outline: 0;
    color: #fff;
    margin: 20px 0;
    display: block;
    width: 100%;
    padding: 5px 0;
    transition: .2s;
    border-bottom:3px solid rgb(199,191,219)
}
.login-container .left-container .input-container input:hover{
    /* cursor: pointer; */
    border-bottom-color: #fff;
}
.login-container .left-container .message-container{
    font-size: 14px;
    transition: .2s;
    color: rgb(199,191,219);
}
.login-container .left-container .message-container:hover{
    color:#fff;
    cursor: pointer;
}
.login-container .right-container{
    display: inline-block;
    width:145px;
    height: 315px;
    vertical-align: top;
    padding: 60px 0;
    position: relative;

}
.login-container .right-container .register-container{
    text-align: center;
    color: #fff;
    font-weight: 200;
    font-size: 18px;
}
.login-container .right-container .register-container span{
    border-bottom: 3px solid rgb(237,221,22);
}
.login-container .right-container .register-container span:hover{
    cursor: pointer;
}
.login-container .right-container .action-container{
    font-size: 14px;
    color: #fff;
    height: 100%;
    text-align: center;
}
.login-container .right-container .action-container span{
    border: 3px solid rgb(237,221,22);
    padding: 10px;
    display: inline-block;
    line-height: 25px;
    border-radius: 25px;
    position: absolute;
    bottom: 60px;
    right: 45px;
    transition: .2s;
}
.login-container .right-container .action-container span:hover{
    background-color: rgb(237,221,22);
    color: rgb(95, 76, 194);
    cursor: pointer;
}
</style>