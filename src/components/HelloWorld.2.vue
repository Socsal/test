<template>
  <div class="a">
    <div class="phoneNum">
      <img :src="phoneNumberIcon" alt="手机号" class="phoneNumIcon">
      <input type="text" class="phoneNumInput">
      <button class="phoneNumBtn">获取验证码</button>
    </div>
    <div class="password">
      <img :src="passwordIcon" alt="密码" class="passwordIcon">
      <input type="text" class="passwordInput">
    </div>
    <div>
      <button class="login">登录</button>
    </div>
    <div class="other">其他登陆方式</div>
    <div class="otherLogin">
      <div>
        <button class="QQLogin">
          <img :src="QQIcon" alt="QQ登录">
        </button>
      </div>
      <div>
        <button class="WeChatLogin">
          <img :src="WeChatIcon" alt="微信登录">
        </button>
      </div>
      <div>
        <button class="WeiboLogin">
          <img :src="WeiboIcon" alt="微博登录">
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>
<style lang="less" scoped>
.a {
  .otherLogin {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    .QQLogin {
      width: 200px;
      height: 200px;
    }
  }
}
</style>


