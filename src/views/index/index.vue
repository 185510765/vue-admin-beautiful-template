<template>
  <div class="index-container">
    <el-row v-if="nodeEnv !== 'development'" :gutter="15">
      <el-col :xs="24" :sm="24" :md="24" :lg="8" :xl="8">
        <el-card>
          <div slot="header">
            开源版本
            <el-button style="float: right; padding: 3px 0;" type="text"
              >永久免费</el-button
            >
          </div>
          <div>
            <ul>
              <li>永久开源免费</li>
              <li>
                开源地址
                <a
                  target="_blank"
                  href="https://github.com/chuzhixin/vue-admin-beautiful"
                  >支持白嫖，也请给个star</a
                >
              </li>
              <li>提供问题讨论群972435319</li>
              <li>
                提供
                <a href="https://chu1204505056.gitee.io/vab-bookmarks/"
                  >讨论群专属文档</a
                >
              </li>
              <li>
                只需保留控制台打印的框架信息即可免费商用
              </li>
            </ul>
            <img src="@/assets/ewm.png" alt="" />
          </div>
        </el-card>
      </el-col>
      <el-col :xs="24" :sm="24" :md="24" :lg="8" :xl="8">
        <el-card>
          <div slot="header">
            商业用途 随意修改版权 提供vip群
            <el-button style="float: right; padding: 3px 0;" type="text"
              >￥299+￥100</el-button
            >
          </div>
          <div>
            <ul>
              <li>支持以上所有特权</li>
              <li>提供VIP讨论群805808910，群主每周定时授课</li>
              <li>
                提供vip群专属文档加群获取，可快速入手框架，并迅速学会脚手架搭建，webpack打包优化
              </li>
              <li>
                可随意变更版权，但仅限自己团队使用，一旦发现恶意传播，二次售卖，不再提供更新支持
              </li>
              <li>你会得到意想不到的回报</li>
              <li>QQ咨询 1204505056</li>
            </ul>
            <img src="@/assets/ewm_vip.png" alt="" />
          </div>
        </el-card>
      </el-col>
      <!--  <el-col :xs="24" :sm="24" :md="24" :lg="8" :xl="8">
        <el-card>
          <div slot="header">
            商业用途 永久更新维护 免费附带vip群（可加4名员工）
            <el-button style="float: right; padding: 3px 0;" type="text"
              >￥1499</el-button
            >
          </div>
          <div>
            <ul>
              <li>支持以上所有特权</li>
              <li>永久更新</li>
              <li>优先问题解答</li>
              <li>提供低价外包合作机会</li>
            </ul>
            <img src="@/assets/ewm_vip.png" alt="" />
          </div>
        </el-card>
      </el-col> -->
    </el-row>
  </div>
</template>

<script>
export default {
  name: "Index",
  components: {},
  data() {
    return {
      nodeEnv: process.env.NODE_ENV,
    };
  },
  created() {},
  mounted() {},
  methods: {},
};
</script>

<style lang="scss" scoped>
.index-container {
  ::v-deep {
    .el-card__body {
      > div {
        min-height: 70vh;
        padding: 20px;

        > ul {
          > li {
            line-height: 30px;
          }
        }

        > img {
          display: block;
          margin: 40px auto;
          border: 1px solid #dedede;
        }
      }
    }
  }
}
</style>
