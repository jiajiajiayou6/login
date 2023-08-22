<template>
  <div class="hello">
    <div class="left">
      <img
        class="imgers"
        alt="Vue logo"
        src="https://img1.baidu.com/it/u=2794961252,1323137487&fm=253&fmt=auto&app=138&f=PNG?w=500&h=707"
      />
    </div>
    <div class="right">
      <div class="yard">
        <img @click="qr" v-if="qqr==1" class="img" alt="Vue logo" src="../assets/yardey.png" />
        <img @click="qrr" v-if="qqr==2" class="img" alt="Vue logo" src="../assets/yredf.png" />
      </div>
      <div class="coders">
        <img v-if="qqr==2" class="imger" alt="Vue logo" src="../assets/yard.png" />
        <div class="logininput" v-if="qqr==1">
          <h2>ERP管理系统用户登录</h2>
          <input type="text" name id placeholder="请登陆用户名" />
          <input type="text" placeholder="请输入密码" />
          <input type="text" name id placeholder="请输入验证码" />
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "HelloWorld",
  data() {
    return {
      qqr: 1
    };
  },
  props: {
    msg: String
  },
  methods: {
    qr() {
      this.qqr = 2;
    },
    qrr() {
      this.qqr = 1;
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="less">
.hello {
  width: 850px;
  height: 450px;
  background: rgb(255, 255, 255);
  position: relative;
  left: 0;
  bottom: 0;
  top: 0;
  right: 0;
  margin: auto;
  margin-top: 50px;
  border-radius: 10px;
  display: flex;
}
.left {
  width: 55%;
  height: 100%;
  position: relative;
  background: rgb(255, 255, 255);
  border-radius: 10px 0 0 10px;
}
.right {
  width: 45%;
  height: 100%;
  position: relative;
  background: rgb(255, 255, 255);
  border-radius: 0 10px 10px 0;
}
.yard {
  float: right;
  width: 80px;
  height: 85px;
  z-index: 3;
  border-radius: 0 10px 10px 0;
}
.yardr {
  float: right;
  width: 80px;
  height: 85px;
  z-index: 4;
  border-radius: 0 10px 10px 0;
}
.img {
  width: 80px;
  height: 80px;
  border-radius: 0 10px 0 0;
}
.coders {
  width: 100%;
  height: 100%;
  background: rgb(255, 255, 255);
  border-radius: 0 10px 10px 0;
}
.imger {
  width: 200px;
  height: 200px;
  position: absolute;
  left: 0;
  right: 0;
  bottom: 0;
  top: 0;
  margin: auto;
}
.imgers {
  width: 400px;
  height: 400px;
  position: absolute;
  left: 0;
  right: 0;
  bottom: 0;
  top: 0;
  margin: auto;
}
.logininput {
  width: 100%;
  height: 100%;
  line-height: 60px;
}
</style>
