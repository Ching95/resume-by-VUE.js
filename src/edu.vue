<template>
  <div> 
    <p><i class="iconfont">&#x3439;</i><span v-text="time"></span></p>
    <p><i class="iconfont">&#xe65e;</i><a href="http://www.gdut.edu.cn/"><span v-text="university"></span></a></p>
    <p><i class="iconfont">&#xe655;</i><span v-text="major"></span></p>
    <p><i class="iconfont">&#xe629;</i><span v-text="GPA"></span></p>
    <p><i class="iconfont">&#xe724;</i><span v-text="English"></span></p>
  </div>
</template>

<script>
export default {
  data () {
    return {
     time:"2013年至今",
     university:"广东工业大学",
     major:"信息工程",
     GPA:"3.72/5.00",
     English:"CET-6"
     
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
    margin: 5px 1%;
  }
  p i{
    margin-right:5px; 
  }
  @media screen and (max-width:980px){
    p{
      margin: 5px 1%;
      width: 30%;
      display: inline-block;
    }
  }
  @media screen and (max-width:680px){
    p{
      width: 46.4%;
    }
  }
  @media screen and (max-width:450px){
    div{
      font-size: 16px;
    }
  }
</style>