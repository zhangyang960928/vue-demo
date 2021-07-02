<template>
  <div>
     <div class="text marginA displayF flex-directionC justify-contentC align-itemsC">
      <div class="foot-one displayF align-itemsC">
        <div class="font-one-word1">RSS</div>
        <div class="font-one-word2">|</div>
        <div class="font-one-word3">源码地址</div>
      </div>
      <div class="foot-two displayF align-itemsC">CNode 社区为国内最专业的  Node.js 开源技术社区，致力于 Node.js 的技术研究。</div>
      <div class="foot-three displayF align-itemsE">
        <div class="foot-three-word1">服务器搭建在</div>
        <div class="foot-three-word2">
          <img src="../../../assets/images/digitalocean.png" alt="">
        </div>
        <div class="foot-three-word1">，储存赞助商为</div>
        <div class="foot-three-word3">
          <img src="../../../assets/images/qiniu.png" alt="">
        </div>
      </div>
      <div class="foot-four displayF align-itemsC">
        <div class="font-four-word1">新手搭建 Node.js 服务器，推荐使用无需备案的</div>
        <div class="font-four-word2">
          <a href="">DigitalOcean(https://www.digitalocean.com/)</a> 
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: '',
  props:{},
  data () {
    return {
    }
  },
  components: {},
  methods: {},
  mounted() {},
  computed: {},
  watch: {}
}
</script>

<style lang='scss' scoped>
.text {
  width: 90%;
  height: 194.54px;
}
.foot-one {
  width: 100%;
  height: 25.6px;
}
.font-one-word1 {
  font-size: 13px;
  color: #666666;
  margin-right: 8px;
}
.font-one-word2 {
  font-size: 13px;
  color: #ABABAB;
  margin-right: 8px;
}
.font-one-word3 {
  font-size: 13px;
  color: #666666;
}
.foot-two {
  width: 100%;
  height: 20px;
  color: #ABABAB;
  font-size: 14px;
  margin-bottom: 10px;
}
.foot-three {
  width: 100%;
  height: 58.94px;
  margin-bottom: 10px;
}
.foot-three-word1 {
  font-size: 14px;
  color: #ABABAB;
}
.foot-three-word2 img {
  width: 92px;
  height: 58.94px;
}
.foot-three-word3 img {
  width: 115px;
  height: 53.66px;
}
.foot-four {
  width: 100%;
  height: 20px;
  color: #ABABAB;
  font-size: 14px;
  margin-bottom: 10px;
}
.font-four-word2 {
  font-size: 14px;
}
.font-four-word2 a {
  text-decoration: none;
  color: #0088cc;
}
.font-four-word2:hover a {
  cursor: pointer;
  text-decoration: underline;
  color: #0055a1;
}
</style>