<template>
  <div>
    <div class="text marginA displayF justify-contentB align-itemsC">
      <!-- 左边部分 -->
      <div class="head-left displayF align-itemsC">
        <div class="head-left-one displayF align-itemsC">
          <img src="../../../assets/images/微信图片_20210609173808.png" alt="" />
        </div>
        <div class="head-left-two displayF align-itemsC">
          <i class="iconfont icon-SearchGlyph"></i>
          <input type="" name="" value="" />
        </div>
      </div>
      <!-- 右边部分 -->
      <div class="head-right displayF justify-contentC align-itemsC">
        <div class="head-right-word">首页</div>
        <div class="head-right-word">新手入门</div>
        <div class="head-right-word">API</div>
        <div class="head-right-word">关于</div>
        <div class="head-right-word" id="quit">退出</div>
        <div class="head-right-word">登录</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "",
  props: {},
  data() {
    return {};
  },
  components: {},
  methods: {},
  mounted() {},
  computed: {},
  watch: {},
};
</script>

<style lang='scss' scoped>
.text {
  width: 90%;
  height: 50px;
}
.head-left {
  width: 393px;
  height: 50px;
}
.head-left-one {
  width: 140px;
  height: 50px;
}
.head-left-one:hover {
  cursor: pointer;
}
.head-left-one img {
  width: 120px;
  height: 28px;
}
.head-left-two {
  width: 233px;
  height: 26px;
  border-radius: 13px;
  background: #888888;
}
.icon-SearchGlyph {
  font-size: 13px;
  margin-left: 10px;
  color: #5c5d5c;
  font-weight: bold;
}
input {
  width: 200px;
  height: 22px;
  background: #888888;
  border: 0px;
}
.head-left-two:hover {
  background: #ffffff;
}
.head-left-two:hover input {
  background: #ffffff;
}
.head-right {
  height: 40px;
}
.head-right-word {
  font-size: 13px;
  color: #cccccc;
  margin: 0px 15px;
}
.head-right:hover {
  cursor: pointer;
}
.head-right-word:hover {
  color: white;
}
</style>