<template>
  <div> 
    <p v-for="skill in skillList"><i class="iconfont">&#xe7d0;</i><span>{{skill.text}}</span></p>
  </div>
</template>

<script>
export default {
  data () {
    return {
     skillList:[
     {text:"掌握语义化的HTML（5）与模块化的CSS（3）"},
     {text:"掌握原生JS编程、Ajax交互技术及jQuery的使用"},
     {text:"了解Bootstrap、vue.js及requireJS、thymeleaf的使用"},
     {text:"了解各浏览器的特性和兼容，有移动端页面开发经验"},
     {text:"熟悉C语言,能使用SublimeText、HBuilder 、PhotoShop等软件"}
     ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  div{
    margin-top: 20px;
    font-size: 18px;
  }
  p{
    margin: 5px;
  }
  p i{
    margin-right:5px; 
  }
  @media screen and (max-width:450px){
    div{
      font-size: 16px;
    }
  }
</style>