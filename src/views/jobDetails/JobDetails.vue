<template>
  <div>
    <div class="wrap">
      <div class="job">
        <div class="name">Java开发工程师</div>
        <div class="salary">0.8-1万/月</div>
      </div>
      <div class="flex">
        <div class="item">
          <img src="./images/nature.png" alt />
          全职
        </div>
        <div class="item">
          <img src="./images/time.png" alt />3-5年
        </div>
        <div class="item">
          <img src="./images/record.png" alt />大专
        </div>
      </div>
      <div class="compan-address">
        <div class="address">
          <img src="./images/address.png" alt />
        </div>
        <div class="address-info">广州市海珠区蚝壳街17号“1号汇创”A座203a</div>
      </div>
      <div class="hr">
        <div class="avatar">
          <img src="../../assets/images/avatar.png" alt />
        </div>
        <div class="hr-info">
          <div class="name">
            陈小街基
            <span class="job-name">人事经理</span>
          </div>
          <p class="conpany">广州市志在信息科技有限公司</p>
        </div>
        <div class="right">
          <img src="./images/right.png" alt />
        </div>
      </div>
    </div>
    <!-- 职责描述 -->
    <div class="instruction">
      <div class="title">
        <img src="../../assets/images/title.png" alt />职位描述
      </div>
      <p class="desc">
        职责描述：
        <br />1、根据业务要求，进行系统的功能设计和逻辑处理；
        <br />2、独立的完成业务系统应用逻辑的开发、并确保开发质量并确保开发质。
        <br />任职要求：
        <br />1、计算机相关专业，本科及以上学历，三年以上java工作经验，对JVM原理有一定的了解
        <br />
      </p>
    </div>

    <!-- 职位福利 -->
    <div class="instruction">
      <div class="title">
        <img src="./images/title.png" alt />职位福利
      </div>
      <div class="welf">
        <div class="green">福利标签</div>
        <div class="skyle">福利标签</div>
        <div class="green">福利标签</div>
      </div>
    </div>
    <!-- 公司信息 -->
    <div class="instruction">
      <div class="title">
        <img src="./images/title.png" alt />公司信息
      </div>
      <!-- 头部 -->
      <div class="list">
        <div class="compnay-info">
          <div class="logo">
            <img src="../../assets/images/company-logo.png" alt />
          </div>
          <div class="info">
            <div class="name">广州市志在信息科技有限公司</div>
            <div class="nature">
              <span>民营企业</span>
              <span>少于50人</span>
              <span>互联网公司</span>
            </div>
            <div class="interviewing">
              在招职位
              <span>22</span>个
            </div>
          </div>
          <div class="right">
            <img src="./images/right.png" alt />
          </div>
        </div>
      </div>
    </div>

    <div class="footer">
      <div class="back" @click="back">
        <div class="my-img">
          <img src="./images/back.png" alt />
        </div>
        <div class="title"> 返回</div>
      </div>
      <div class="back">
        <div class="my-img">
          <img src="./images/share.png" alt />
        </div>
        <div class="title">分享</div>
      </div>
      <div class="back">
        <div class="my-img">
          <img src="./images/collect.png" alt />
        </div>
        <div class="title">收藏</div>
      </div>
      <div class="save">立即投递</div>
    </div>
  </div>
</template>

<script>
export default {
  name: "CompanyInfo",
  methods: {
    back() {
      this.$router.push("./home");
    },
    // 去在招职位
    toRecruit() {
      console.log("7777");
      this.$router.push("/recruit");
    }
  }
};
</script>

<style lang="scss" scoped>
.wrap {
  width: 6.9rem;
  margin: auto;
  padding: 0.2rem 0.1rem;
  box-sizing: border-box;
  overflow: hidden;
  box-shadow: 0 0.05rem 0.3rem #fff1ea;
  .job {
    display: flex;
    justify-content: space-between;
    line-height: 0.6rem;
    .name {
      font-size: 0.34rem;
      color: #323232;
    }
    .salary {
      font-size: 0.36rem;
      color: #e81010;
    }
  }
  .flex {
    display: flex;
    line-height: 0.5rem;
    .item {
      width: 1.5rem;
      font-size: 0.28rem;
      color: #9a9a9a;
      img {
        width: 0.24rem;
        margin-right: 0.1rem;
      }
    }
  }
  .compan-address {
    display: flex;
    line-height: 0.5rem;
    padding-bottom: 0.1rem;
    border-bottom: 0.02rem solid #f0f0f0;
    box-sizing: border-box;
    .address {
      width: 0.2rem;
      overflow: hidden;
      margin-right: 0.2rem;
      img {
        width: 100%;
        display: block;
        margin-top: 0.04rem;
      }
    }
    .address-info {
      font-size: 0.28rem;
      color: #9a9a9a;
    }
  }
  .hr {
    display: flex;
    position: relative;
    width: 100%;
    margin-top: 0.1rem;
    .avatar {
      width: 0.8rem;
      margin-right: 0.2rem;
      margin-top: 0.1rem;
      img {
        width: 100%;
        display: block;
      }
    }
    .hr-info {
      line-height: 0.46rem;
      .name {
        font-size: 0.32rem;
        .job-name {
          font-size: 0.24rem;
          padding: 0 0.1rem;
          background: #fff1ea;
          color: #ffa277;
          margin-left: 0.2rem;
        }
      }
      .conpany {
        font-size: 0.28rem;
        color: #9a9a9a;
      }
    }
    .right {
      width: 0.2rem;
      position: absolute;
      top: 0.28rem;
      right: 0;
      img {
        display: block;
        width: 100%;
      }
    }
  }
}
.instruction {
  width: 100vw;
  padding: 0 0.3rem;
  box-sizing: border-box;
  .title {
    font-size: 0.32rem;
    color: #323232;
    margin: 0.2rem 0;
    letter-spacing: 0.04rem;
    img {
      width: 0.24rem;
      height: 0.24rem;
      margin-right: 0.2rem;
    }
  }
  .desc {
    font-size: 0.28rem;
    color: #9a9a9a;
    line-height: 0.42rem;
  }
  .welf {
    display: flex;
    div {
      padding: 0 0.2rem;
      font-size: 0.24rem;
      line-height: 0.32rem;
      border: 1px solid;
      margin-right: 0.2rem;
    }
    .green {
      border-color: #6adea0;
      color: #6adea0;
    }
    .skyle {
      border-color: #6ba2fd;
      color: #6ba2fd;
    }
  }
  .list {
    width: 100%;
    .compnay-info {
      display: flex;
      position: relative;
      padding-bottom: 0.1rem;
      box-sizing: border-box;
      .logo {
        width: 1rem;
        margin-right: 0.2rem;
        margin-top: 0.4rem;
        img {
          display: block;
          width: 100%;
        }
      }
      .info {
        width: 5rem;
        .name {
          font-size: 0.28rem;
          color: #323232;
          margin-top: 0.3rem;
        }
        .nature {
          line-height: 0.6rem;
          display: flex;
          flex-wrap: nowrap;
          position: relative;
          span {
            display: block;
            font-size: 0.28rem;
            color: #9a9a9a;
            position: relative;
            margin-right: 0.2rem;
            &:last-of-type {
              &::after {
                background: transparent;
              }
            }
            &::after {
              position: absolute;
              top: 0.18rem;
              right: -0.1rem;
              content: "";
              width: 0.03rem;
              height: 0.23rem;
              background: #ccc;
            }
          }
        }
        .interviewing {
          font-size: 0.28rem;
          color: #9a9a9a;
          span {
            color: $font-color;
            margin: 0 0.1rem;
          }
        }
      }
      .right {
        position: absolute;
        right: 0;
        top: 0.5rem;
        width: 0.15rem;
        img {
          display: block;
          width: 100%;
        }
      }
    }
  }
}
.footer {
  width: 100vw;
  padding: 0 .3rem;
  box-sizing: border-box;
  display: flex;
  height: 1rem;
  position: fixed;
  bottom: 0;
  left: 0;
  background: #fff;
  overflow: hidden;
  border-top: 1px solid #ccc;
  .back {
    width: .8rem;
    margin-right: .3rem;
    margin-top: .2rem;
    .my-img {
      width: .3rem;
      margin: auto;
      height: .4rem;
      overflow: hidden;
      img {
        display: block;
        width: 100%;
      }
    }
    .title {
      width: 100%;
      text-align: center;
      color: #323232;
      font-size: .28rem;
    }
  }
  .save {
    flex: 1;
    font-size: .36rem;
    text-align: center;
    color: #fff;
    margin-top: .16rem;
    line-height: .7rem;
    height: .7rem;
    border-radius: .1rem;
    background-image: linear-gradient(to right, #FFB246, #FF8853);
  }
}
</style>