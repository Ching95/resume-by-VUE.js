<template>
    <dl>
     <div v-for="campus in campusList">
      <dt><i class="iconfont">&#xe65f;</i><span>{{campus.time}}</span><b>{{campus.title}}</b></dt>
      <dd><span>{{campus.content}}</span></dd>
      
     </div>
    </dl>
</template>

<script>
export default {
  data () {
    return {
     campusList:[
      {time:"2014.09~2015.06",
        title:"院学生会学习部正部长",
        content:"学风活动举办和部门管理，培养协调管理能力、锻炼沟通交流能力、提升执行力，获学生会优秀干部称号"
      },
      {time:"2013.09~2014.06",
        title:"副班长/年级级委",
        content:"管理班级事务和年级事务，促进跟同学之间的融洽相处，培养认真负责的工作态度，获优秀班干部称号。"
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
  dt b{
    margin-left: 5%;
  }
  @media screen and (max-width:450px){
    dl{
      font-size: 16px;
    }
    dt b{
      display: block;
      margin-left:20px;
    }
  }
</style>