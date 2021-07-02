<template>
  <div>
    <div class="text marginA displayF justify-contentB">
      <!-- 左边部分 -->
      <div class="body-left">
        <!-- 固定部分 -->
        <div class="body-left-word1 displayF align-itemsC">
          <div class="body-left-word1-box">全部</div>
          <div class="body-left-word1-box">精华</div>
          <div class="body-left-word1-box">分享</div>
          <div class="body-left-word1-box">问答</div>
          <div class="body-left-word1-box">招聘</div>
          <div class="body-left-word1-box">客户端测试</div>
        </div>
        <!-- 引入部分 -->
        <div class="body-left-word2" v-for="(item, index) in list" :key="index">
          <div class="flex">
            <!-- 图片 -->
            <div>
              <img :src="item.author.avatar_url" class="avatar" />
            </div>
            <!-- 访问数 -->
            <div class="div2">
              <div class="reply">
                {{ item.reply_count }}
                <div id="one">/</div>
              </div>
              <div class="visit">
                {{ item.visit_count }}
              </div>
            </div>
            <!-- 置顶 -->
            <div>
              <div class="top" v-if="index < 3">置顶</div>
              <div class="tab" v-if="index > 2 && item.tab === 'share'">
                分享
              </div>
              <div class="tab" v-if="index > 2 && item.tab === 'ask'">回答</div>
            </div>
            <!-- 内容 -->
            <div class="div4">
              <div class="title">
                {{ item.title }}
              </div>
            </div>
            <!-- 时间 -->
            <div class="div5">
              <div class="create">
                {{ item.create }}
              </div>
            </div>
          </div>
        </div>
      </div>
      <!-- 右边部分 -->
      <div class="body-right">
        <!-- 右边第一个盒子 也就是登录前的盒子-->
        <div
          class="body-right-word1 displayF flex-directionC justify-contentC align-itemsC"
        >
          <!-- 第一层盒子 -->
          <div class="body-right-word1-box1 displayF align-itemsC">
            CNode：Node.js专业中文社区
          </div>
          <!-- 第二层盒子 -->
          <div class="body-right-word1-box2 displayF flex-directionC">
            <!-- 第二层盒子内容 -->
            <div class="body-right-word1-box2-content1 displayF align-itemsC">
              <div class="body-right-word1-box2-content1-one">您可以&nbsp;</div>
              <div class="body-right-word1-box2-content1-two">登录</div>
              <div class="body-right-word1-box2-content1-one">
                &nbsp;或&nbsp;
              </div>
              <div class="body-right-word1-box2-content1-two">注册</div>
              <div class="body-right-word1-box2-content1-one">
                &nbsp;，也可以
              </div>
            </div>
            <div
              class="body-right-word1-box2-content2 displayF justify-contentC align-itemsC"
            >
              通过 GitHub 登录
            </div>
          </div>
        </div>
        <!-- 登录后的盒子 -->
        <div
          class="body-right-word1-sign displayF flex-directionC justify-contentC align-itemsC"
        >
          <div class="body-right-word1-sign-word1"></div>
          <div class="body-right-word1-sign-word2">积分：960</div>
          <div class="body-right-word1-sign-word3">
            “狼叔说：少抱怨，多思考，未来更美好”
          </div>
        </div>
        <!-- 右边第二个盒子 -->
        <div class="body-right-word2">
          <!-- 第一层 -->
          <div class="body-right-word2-box1 displayF align-itemsC">
            <div class="body-right-word2-box1-one">无人回复的话题</div>
          </div>
          <!-- 第二层 -->
          <div
            class="body-right-word2-box2 displayF flex-directionC justify-contentC align-itemsC"
          >
            <div class="body-right-word2-box2-content">
              【pomelo】master服务和connector等服务的创建流程
            </div>
            <div class="body-right-word2-box2-content">
              使用 Socket.IO 进行授权和握手
            </div>
            <div class="body-right-word2-box2-content">
              是否可以使用nginx转发websocket实现Node远程调试？
            </div>
            <div class="body-right-word2-box2-content">
              typescript+nodejs报错：Cannot redeclare block
            </div>
            <div class="body-right-word2-box2-content">
              现在firefox的更新是不是在更新tab?
            </div>
          </div>
        </div>
        <!-- 右边第三个盒子 -->
        <div class="body-right-word3">
          <!-- 第一层 -->
          <div class="body-right-word3-box1 displayF align-itemsC">
            <div class="body-right-word3-box1-content1">积分榜</div>
            <div class="body-right-word3-box1-content2">TOP 100 >></div>
          </div>
          <!-- 第二层 -->
          <div
            class="body-right-word3-box2 displayF flex-directionC justify-contentC align-itemsC"
          >
            <div class="body-right-word3-box2-content displayF align-itemsC">
              <div class="body-right-word3-box2-content1">22720</div>
              <div class="body-right-word3-box2-content2">i5ting</div>
            </div>
            <div class="body-right-word3-box2-content displayF align-itemsC">
              <div class="body-right-word3-box2-content1">15840</div>
              <div class="body-right-word3-box2-content2">alsotang</div>
            </div>
            <div class="body-right-word3-box2-content displayF align-itemsC">
              <div class="body-right-word3-box2-content1">10045</div>
              <div class="body-right-word3-box2-content2">atian25</div>
            </div>
            <div class="body-right-word3-box2-content displayF align-itemsC">
              <div class="body-right-word3-box2-content1">9350</div>
              <div class="body-right-word3-box2-content2">leapon</div>
            </div>
            <div class="body-right-word3-box2-content displayF align-itemsC">
              <div class="body-right-word3-box2-content1">8780</div>
              <div class="body-right-word3-box2-content2">jiyinyiyong</div>
            </div>
            <div class="body-right-word3-box2-content displayF align-itemsC">
              <div class="body-right-word3-box2-content1">7800</div>
              <div class="body-right-word3-box2-content2">yakczh</div>
            </div>
            <div class="body-right-word3-box2-content displayF align-itemsC">
              <div class="body-right-word3-box2-content1">6855</div>
              <div class="body-right-word3-box2-content2">im-here</div>
            </div>
            <div class="body-right-word3-box2-content displayF align-itemsC">
              <div class="body-right-word3-box2-content1">6135</div>
              <div class="body-right-word3-box2-content2">DevinXian</div>
            </div>
            <div class="body-right-word3-box2-content displayF align-itemsC">
              <div class="body-right-word3-box2-content1">5815</div>
              <div class="body-right-word3-box2-content2">chapgaga</div>
            </div>
            <div class="body-right-word3-box2-content displayF align-itemsC">
              <div class="body-right-word3-box2-content1">5375</div>
              <div class="body-right-word3-box2-content2">magicdawn</div>
            </div>
          </div>
        </div>
        <!-- 右边第四个盒子 -->
        <div class="body-right-word4">
          <div class="body-right-word4-box1 displayF align-itemsC">
            <div class="body-right-word4-box1-content">友情社区</div>
          </div>
          <div
            class="body-right-word4-box2 displayF flex-directionC justify-contentC align-itemsC"
          >
            <div class="body-right-word4-box2-content">
              <img
                src="../../../assets/images/ruby-china-20150529.png"
                alt=""
              />
            </div>
            <div class="body-right-word4-box2-content">
              <img src="../../../assets/images/golangtc-logo.png" alt="" />
            </div>
            <div class="body-right-word4-box2-content">
              <img src="../../../assets/images/phphub-logo.png" alt="" />
            </div>
          </div>
        </div>
        <!-- 右边第五个盒子 -->
        <div class="body-right-word5">
          <div class="body-right-word5-box1 displayF">
            <div class="body-right-word5-box1-content displayF align-itemsC">
              客户端二维码
            </div>
          </div>
          <div
            class="body-right-word5-box2 displayF flex-directionC justify-contentC align-itemsC"
          >
            <div class="body-right-word5-box2-content1">
              <img
                src="../../../assets/images/FtG0YVgQ6iginiLpf9W4_ShjiLfU.png"
                alt=""
              />
            </div>
            <div class="body-right-word5-box2-content2">客户端源码地址</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import axios from "axios";
import dayjs from "dayjs";
export default {
  name: "",
  props: {},
  data() {
    return {
      list: [],
    };
  },
  components: {},
  methods: {
    getData() {
      axios
        .get("https://cnodejs.org/api/v1/topics")
        .then((res) => {
          console.log(res.data.data);
          this.list = res.data.data;
          this.list.map((item) => {
            let time = dayjs().valueOf();
            let timer = dayjs(item.create_at).valueOf();
            let t = time - timer;
            let s = Math.floor((t / 1000) % 60);
            let f = Math.floor((t / 1000 / 60) % 60);
            let h = Math.floor((t / 1000 / 60 / 60) % 24);
            let d = Math.floor((t / 1000 / 60 / 60 / 24) % 24);
            if (h > 0 && d === 0) {
              item.create = h + "小时之前";
            } else if (d > 0) {
              item.create = d + "天之前";
            }
          });
        })
        .catch((err) => {
          console.log("请求失败", err);
        });
    },
  },
  mounted() {
    this.getData();
  },
  computed: {},
  watch: {},
};
</script>

<style lang='scss' scoped>
.text {
  width: 90%;
  margin-top: 15px;
}
.body-right {
  width: 290px;
}
.body-right-word1 {
  width: 290px;
  height: 115.2px;
  background: #ffffff;
  margin-bottom: 13px;
  border-radius: 2px;
  display: none;
}
.body-right-word1-box1 {
  width: 270px;
  height: 25.6px;
  color: #333333;
  font-size: 14px;
  margin-bottom: 10px;
  padding: 10px 0px 0px 10px;
}
.body-right-word1-box2 {
  width: 270px;
  height: 59.6px;
  padding-left: 10px;
}
.body-right-word1-box2-content1 {
  width: 270px;
  height: 25.6px;
  color: #333333;
  font-size: 13px;
}
.body-right-word1-box2-content1-two {
  color: #778087;
}
.body-right-word1-box2-content1-two:hover {
  cursor: pointer;
  text-decoration: underline;
}
.body-right-word1-box2-content2 {
  width: 150.99px;
  height: 34px;
  background: #5bc0de;
  border-radius: 3px;
  color: #ffffff;
  font-size: 14px;
}
.body-right-word1-box2-content2:hover {
  cursor: pointer;
}
.body-right-word2 {
  width: 290px;
  height: 218px;
  background: #ffffff;
  margin-bottom: 13px;
  border-radius: 2px;
}
.body-right-word2-box1 {
  width: 290px;
  height: 40px;
  background: #f6f6f6;
  color: #51585c;
  font-size: 13px;
  border-top-left-radius: 2px;
  border-top-right-radius: 2px;
}
.body-right-word2-box1-one {
  margin-left: 10px;
}
.body-right-word2-box2 {
  width: 290px;
  height: 178px;
}
.body-right-word2-box2-content {
  width: 270px;
  height: 29.6px;
  color: #778087;
  font-size: 14px;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
  line-height: 29.6px;
}
.body-right-word3 {
  width: 290px;
  height: 336.5px;
  background: white;
  margin-bottom: 13px;
}
.body-right-word3-box1 {
  width: 290px;
  height: 40px;
  background: #f6f6f6;
}
.body-right-word3-box1-content1 {
  font-size: 13px;
  color: #444444;
  margin-left: 10px;
}
.body-right-word3-box1-content2 {
  font-size: 13px;
  color: #666666;
  margin-left: 10px;
}
.body-right-word3-box1-content2:hover {
  cursor: pointer;
}
.body-right-word3-box2 {
  width: 290px;
  height: 296.5px;
}
.body-right-word3-box2-content {
  width: 270px;
  height: 26.85px;
}
.body-right-word3-box2-content1 {
  color: #808080;
  font-size: 13px;
  margin-right: 10px;
  padding: 2px;
}
.body-right-word3-box2-content2 {
  color: #778087;
  font-size: 13px;
}
.body-right-word3-box2-content2:hover {
  cursor: pointer;
  text-decoration: underline;
}
.body-right-word4 {
  width: 290px;
  height: 220.4px;
  margin-bottom: 13px;
  background-color: white;
}
.body-right-word4-box1 {
  width: 290px;
  height: 40px;
  color: #444444;
  font-size: 13px;
  background: #f6f6f6;
}
.body-right-word4-box1-content {
  margin-left: 10px;
}
.body-right-word4-box2 {
  width: 290px;
  height: 180.4px;
}
.body-right-word4-box2-content {
  margin-bottom: 10px;
  width: 270px;
  height: 49.51px;
}
.body-right-word4-box2-content img {
  width: 150px;
  height: 49.51px;
}
.body-right-word4-box2-content img:hover {
  cursor: pointer;
}
.body-right-word5 {
  width: 290px;
  height: 285.6px;
  background: white;
  margin-bottom: 13px;
}
.body-right-word5-box1 {
  width: 290px;
  height: 40px;
  background: #f6f6f6;
  color: #51585c;
  font-size: 13px;
}
.body-right-word5-box1-content {
  margin-left: 10px;
}
.body-right-word5-box2-content1 img {
  width: 200px;
  height: 200px;
}
.body-right-word5-box2 {
  width: 290px;
  height: 245.6px;
}
.body-right-word5-box2-content2 {
  color: #778087;
  font-size: 13px;
}
.body-right-word5-box2-content2:hover {
  cursor: pointer;
}
.body-left-word1 {
  width: 1062.28px;
  height: 40px;
  color: #333333;
  font-size: 14px;
  background: #f6f6f6;
}
.body-left-word1-box {
  color: #80bd01;
  font-size: 14px;
  margin: 0px 10px;
  padding: 3px 4px;
}
.body-left-word1-box:hover {
  background: #80bd01;
  color: white;
  cursor: pointer;
}
.body-left-word2 {
  width: 1062.28px;
}
.flex {
  display: flex;
  width: 1052.28px;
  height: 50.39px;
  align-items: center;
  padding-left: 10px;
  background: white;
  position: relative;
  border-bottom: 1px #f6f6f6 solid;
}
.flex:hover {
  background: #f6f6f6;
}
.avatar {
  width: 30px;
  height: 30px;
}
.avatar:hover {
  cursor: pointer;
}
.div2 {
  display: flex;
  align-items: center;
  justify-content: center;
  margin-left: 5px;
  width: 70px;
}
.reply {
  color: #9e78c0;
  font-size: 14px;
  display: flex;
}
#one {
  color: black;
  margin: 0px 2px;
}
.visit {
  color: #b4b4b4;
  font-size: 12px;
}
.top {
  color: #ffffff;
  background: #80bd01;
  padding: 2px 4px;
  font-size: 12px;
  border-radius: 3px;
  margin-left: 3px;
}
.tab {
  color: #999;
  background: #e5e5e5;
  padding: 2px 4px;
  font-size: 12px;
  border-radius: 3px;
  margin-left: 3px;
}
.title {
  color: #333;
  font-size: 16px;
  margin-left: 3px;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
  width: 729.59px;
}
.title:hover {
  cursor: pointer;
  text-decoration: underline;
}
.create {
  font-size: 12px;
  color: #778087;
}
.div5 {
  position: absolute;
  right: 10px;
}
.create:hover {
  cursor: pointer;
}
.body-right-word1-sign {
  width: 290px;
  height: 115.2px;
  background: #ffffff;
  margin-bottom: 13px;
  border-radius: 2px;
  display: none;
}
.body-right-word1-sign-word1 {
  font-size: 20px;
  color: #778087;
  padding: 20px 0px 0px 20px;
}
.body-right-word1-sign-word2 {
  font-size: 12px;
  color: #778087;
  padding: 10px 0px 0px 20px;
}
.body-right-word1-sign-word3 {
  font-size: 12px;
  color: #778087;
  padding: 10px 0px 0px 20px;
  font-style: italic;
}
</style>