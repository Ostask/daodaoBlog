<template>
  <div class="container">
    <div class="left">
      <div class="part">
        <div class="title">个人作品</div>
        <div class="person-work">
          <div class="card" v-for="i in 8" :key="i+'card'">
            <div class="img-content">
              <img src="https://i0.hdslb.com/bfs/archive/0cdcdb2fe67dd860d56a29c73b399531130cc8cb.jpg@206w_116h_1c_100q.jpg" alt="">
            </div>
            <div class="work-title">我的作品之一</div>
            <div class="user">刀刀</div>
          </div>
        </div>
      </div>

      <div class="part">
        <div class="title">热门文章</div>
        <div class="article-list">
            <div class="article" v-for="i in 5" :key="i">
                <div class="user-info">
                  <span class="tag">原创</span>
                  <span class="tag" style="margin-left:2px;">分类类型</span>
                  <span class="user">刀刀</span>
                  <span class="create-time">4天前</span>
                  <span class="read">
                      阅读:3
                  </span>
                  <span class="message">
                      留言:1
                  </span>
                  <span class="star">
                      点赞:100
                  </span>
                </div>
                <div class="article-title">element-ui的table在flex布局下宽度一直增大的问题，解决了！！解决了！！</div>
                <div class="pre-read">
                  导读：写这篇文章的主要目的就是把自己学过的知识进行梳理，整个的学习路线是我自己对技术的一个学习规划，向着每一个程序员的终极目标而努力！对象：Java初/中/高级程序员开始：2020-07-20结束：生命不息，学习不止！目录【入门篇】【基础篇】【系统篇】【数据库】【服务器】【进阶篇】【前端
                </div>
            </div>
        </div>
      </div>

      <div class="part">
        <div class="title">最新文章</div>
        <div class="article-list">
            <div class="article" v-for="i in 5" :key="i">
                <div class="user-info">
                  <span class="tag">原创</span>
                  <span class="tag" style="margin-left:2px;">分类类型</span>
                  <span class="user">刀刀</span>
                  <span class="create-time">4天前</span>
                  <span class="read">
                      阅读:3
                  </span>
                  <span class="message">
                      留言:1
                  </span>
                  <span class="star">
                      点赞:100
                  </span>
                </div>
                <div class="article-title">element-ui的table在flex布局下宽度一直增大的问题，解决了！！解决了！！</div>
                <div class="pre-read">
                  导读：写这篇文章的主要目的就是把自己学过的知识进行梳理，整个的学习路线是我自己对技术的一个学习规划，向着每一个程序员的终极目标而努力！对象：Java初/中/高级程序员开始：2020-07-20结束：生命不息，学习不止！目录【入门篇】【基础篇】【系统篇】【数据库】【服务器】【进阶篇】【前端
                </div>
            </div>
        </div>
      </div>
    </div>
    <div class="right">

    </div>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.container{
  width:1200px;
  margin:0 auto;
  display: flex;
  .left{
    flex:1;
  }
  .right{
    width:300px;
  }
  .part{
    background: #fff;
    margin:10px;
    border:1px solid rgba(151,151,151,0.1);
    .title{
      color:#91d281;
      font-size:18px;
      border-bottom:1px solid rgba(151,151,151,0.1);
      padding:10px 24px;
    }
    .article-list{
      .article{
        padding:18px 24px;
        &:not(:last-child) {
         border-bottom:1px solid rgba(151,151,151,0.1);
        }
        .user-info{
          font-size:12px;
          color:#676767;
          .tag{
            padding:2px;
            border:1px solid #91d281;
            background: #e5f5e1;
            border-radius: 2px;;
          }
          .user{
            margin-left:2px;
          }
          .create-time{
            margin-left:2px;
          }
          .read{
            margin-left:20px;
          }
        }
        .article-title{
          color:#2e3135;
          font-size:18px;
          font-weight:bold;
          padding:4px;
        }
        .pre-read{
          color:#9a9a9a;
          font-size:14px;
          line-height: 20px;
        }
      }
    }
    .person-work{
      display: flex;
      flex-wrap: wrap;
      padding:18px 24px 28px 14px;
      .card{
        width:25%;
        box-sizing: border-box;
        padding:10px 0 0 10px;
        .img-content{
          height:110px;
          overflow: hidden;
          border-radius: 4px;
          img{
            width:100%;
            min-height:110px;
          }
        }
        .work-title{
          font-size:14px;
          color:#2e3135;
        }
        .user{
          color:#9a9a9a;
          font-size:12px;
        }
      }
    }
  }
}
</style>
