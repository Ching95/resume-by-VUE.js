<template>
<div id="page">
  <section id="infor">
    <h1 v-text="infor"></h1>
    <information></information>
  </section>
  <section id="edu">
    <h1 v-text="edu"></h1>
    <edu></edu>
  </section>
  <section id="skill">
    <h1 v-text="skill"></h1>
    <skill></skill>
  </section>
  <section id="practice">
    <h1 v-text="practice"></h1>
    <practice></practice>
  </section>
  <section id="project">
    <h1 v-text="project"></h1>
    <project></project>
  </section>
  <section id="campus">
    <h1 v-text="campus"></h1>
    <campus></campus>
  </section>
  <section id="award">
    <h1 v-text="award"></h1>
    <award></award>
  </section>
  <section id="eva">
    <h1 v-text="eva"></h1>
    <eva></eva>
  </section>

</div>
  <footer><p>This resume is generated with Gulp and VUE by Ching.<br/>请使用IE8以上的浏览器查看</p></footer>
</template>

<script>
import information from './information';
import edu from './edu';
import skill from './skill';
import practice from './practice';
import project from './project';
import campus from './campus';
import award from './award';
import eva from './eva';
export default {
  data:function () {
    return {
      infor:"个人信息",
      edu:"教育经历",
      skill:"个人技能",
      project:"项目经历",
      practice:"实习经历",
      campus:"校园经历",
      award:"荣誉奖项",
      eva:"自我评价"
    }
  },
  components:{
    information,
    edu,
    skill,
    practice,
    project,
    campus,
    award,
    eva
  }
}
</script>

<style>
  @import '../static/iconfont.css';
  *{
    padding: 0;
    margin:0;
  }
  a{
    text-decoration: none;
    color: #000000;
  }
  a:link{
    color: #000000;
  }
  /*a:visited{
    color:#CD5B45 ;
  }*/
  a:focus,a:hover,a:active{
    color:#9B30FF; 
  }
  html{
    margin: 20px 0;
    background-color: rgb(224,224,224);
  }
  #page{
    width: 80%;
    min-width: 300px;
    margin: 0 auto;
    padding-bottom: 20px;
    border: 1px solid rgb(198,198,198);
    -moz-border-radius: 5px;
    -webkit-border-radius: 5px;
    border-radius: 5px;/*IE<9不支持*/
    -moz-box-shadow: 2px 2px 3px 3px rgb(198,198,198);
    -webkit-box-shadow: 2px 2px 3px 3px rgb(198,198,198);
    box-shadow: 2px 2px 3px 3px rgb(198,198,198);
    background: url(./assets/bg3.jpg) left top repeat;
  }
  #infor,#edu,#skill,#project,#practice,#campus,#award,#eva{
    padding:5px 1%;
    background-color: rgba(255,255,255,.2);
    filter:progid:DXImageTransform.Microsoft.gradient(startColorstr=#33FFFFFF,endColorstr=#33FFFFFF);    /*IE8支持*/
    margin:35px 1% 0px;
    -moz-border-radius: 10px;
    -webkit-border-radius: 10px;
    border-radius: 10px;
    position: relative;
  }
  #edu,#skill,#award,#eva{
    display: inline-block;
    
  }
  #edu{
    width: 29.2%;
  }
  #skill{
    width: 61.5%;
  }
  #award{
    width: 45.5%;
  }
  #eva{
    width: 45.5%;
  }
  h1{
    font-size: 22px;
    padding: 8px;
    -moz-border-radius: 10px;
    -webkit-border-radius: 10px;
    border-radius: 10px;
    background-color: rgba(0,0,0,.8);
    filter:progid:DXImageTransform.Microsoft.gradient(startColorstr=#C8000000,endColorstr=#C8000000);    /*IE8支持*/
    color: rgb(255,255,255);
    position:absolute;
    top:-20px;
    left: 0px
  }
  footer{
    width: 80%;
    margin: 20px auto 0px;
  }
  footer p{
    text-align: center;
    font-weight: lighter;
  }
  @media screen and (max-width:980px){
    #edu,#skill,#award,#eva{
      display: block;
      width: auto;
    }
  }
  
</style>
