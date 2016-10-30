<template>
    <dl>
     <div v-for="project in projectList">
        <dt><i class="iconfont">&#xe60f;</i><span>{{project.title}}</span></dt>
        <dd><p>{{project.titleOne}}</p><span>{{project.content}}</span></dd>
        <dd><p>{{project.titleSec}}</p><span>{{project.experience}}</span></dd>
     </div>
    </dl>
</template>

<script>
export default {
  data () {
    return {
     projectList:[
       {title:"公众号商城团购功能的开发",
        titleOne:"项目介绍",
        content:"包括从团购首页到团分享等页面，用HTML5和CSS3实现页面、jQuery实现页面动态功能，利用thymeleaf及AJAX实现前后端数据交互",
        titleSec:"个人体会",
        experience:"学习新知识并学以致用，接触移动端页面开发，熟悉页面bug的调试方法"
      },
      {title:"本人网页简历的制作",
        titleOne:"项目介绍",
        content:"致力重点突出页面简洁，考虑浏览器兼容性，注重页面结构表现行为分离，便于后期维护",
        titleSec:"个人体会",
        experience:"加深对jQuery的理解运用，同时在页面结构表现行为分离的重要性有了更深的体会"
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
  dt i{
    margin-right: 5px;
  }
  dd p{
    display: inline-block;
    margin-right:10px;
    font-weight: bold;
  }
  @media screen and (max-width:450px){
    dl{
      font-size: 16px;
    }
  }
</style>