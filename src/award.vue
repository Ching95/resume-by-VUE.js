<template>
  <div> 
    <p v-for="award in awardList"><i class="iconfont">&#xe615;</i><span>{{award.text}}</span></p>
  </div>  
</template>

<script>
export default {
  data () {
    return {
     awardList:[
      {text:"校优秀学生二等奖学金（X2）（TOP10%）"},
      {text:"校电子设计竞赛一等奖"},
      {text:"广州大学城校际实验综合技能邀请赛二等奖"},
      {text:"全国电子设计竞赛（广东赛区）成功参赛奖"}
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
    margin-right: 5px;
  }
  @media screen and (max-width:450px){
    div{
      font-size: 16px;
    }
  }
</style>