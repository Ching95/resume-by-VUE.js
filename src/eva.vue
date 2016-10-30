<template>
  <div> 
    <p v-for="eva in evaList"><i class="iconfont">&#xe620;</i><span>{{eva.text}}</span></p>
  </div>  
</template>

<script>
export default {
  data () {
    return {
     evaList:[
      {text:"学习能力较强，有求知欲"},
      {text:"对前端充满热情，具备较好的理解能力。"},
      {text:"对待工作认真负责，吃苦耐劳，愿意坚持"},
      {text:"积极乐观，性格随和易相处，协作合作能力好"},
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