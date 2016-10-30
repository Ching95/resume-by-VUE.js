<template>
    <dl>
      <div v-for="practice in practiceList">
        <dt><i class="iconfont">&#xe602;</i><span>{{practice.company}}</span><span class="bPosition"><span class="jobPosition">{{practice.position}}</span><span>{{practice.time}}</span></span></dt>
        <dd><p>{{practice.titleOne}}</p><span>{{practice.content}}</span></dd>
        <dd><p>{{practice.titleSec}}</p><span>{{practice.participate}}</span></dd>
      </div>
    </dl>
</template>

<script>
export default {
  data () {
    return {
     practiceList:[
       {company:"广州市蓝栈信息科技有限公司",
        position:"前端实习生",
        time:"2016.07~至今",
        titleOne:"实习内容",
        content:"学习MUI框架、requireJS，优化web App页面；学习thymeleaf模板，根据设计图开发新页面。",
        titleSec:"参与项目",
        participate:"城全记WEB APP的优化、邻里服务家公众号商城团购功能的开发"
      },
      {company:"广州市博丽信息科技有限公司",
        position:"前端实习生",
        time:"2016.05~2016.07",
        titleOne:"实习内容",
        content:"学习Bootstrap，利用模板制作网站；根据设计图使用 HTML、CSS、JS实现页面，优化他人制作的页面。",
        titleSec:"参与项目",
        participate:"公司官网的制作、清风扶绥网的制作"
      }
     ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  dl{
    margin-top: 20px;
    font-size: 18px;
  }
  dt,dd{
    margin: 5px;
  }
  .jobPosition{
    margin:0 7%; 
  }
  dt i{
    margin-right: 5px;
  }
  dd p{
    display: inline-block;
    margin-right:10px;
    font-weight: bold;
  }
  @media screen and (max-width:680px){
    .bPosition{
      display: block;
      
    }
    .jobPosition{
      margin:0 7% 0 18px; 
    }
  }
  @media screen and (max-width:450px){
    dl{
      font-size: 16px;
    }
  }
</style>