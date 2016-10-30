<template>
  <div> 
    <div class="inforWho">
      <h2 class="name" v-text="name"></h2>
      <h3 class="job" v-text="job"></h3>
    </div>
    <div class="inforDetail">
      <p><i class="iconfont">&#xe60c;</i><a href="tel:18813756654" v-text="phone"></a></p>
      <p><i class="iconfont">&#xe61f;</i><a href="mailto:1149533970@qq.com" v-text="mail"></a></p>
      <p><i class="iconfont">&#xe735;</i><a href="https://github.com/Ching95" v-text="gitHub"></a></p>   
    </div>
    <!-- <img v-bind:src="src" /> -->
    <img src="assets/ching.jpg">
  </div>
</template>

<script>
export default {
  data () {
    return {
     name:"林城青",
     job:"前端开发工程师",
     phone:"18813756654",
     mail:"1149533970@qq.com",
     gitHub:"https://github.com/Ching95",
     // src:"./assets/ching.jpg"
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

  .inforWho{
   display: inline-block;
   width: 24%;
  }
  .name{
    margin: 30px 0 0px;
    font-size: 35px;
    text-align: center;
  }
  .job{
    margin: 15px 0;
    font-size: 25px;
    text-align: center;
  }
  .inforDetail{
   display: inline-block;
   width: 30%;
   font-size: 22px;
   margin-left: 10%;
  }
  .inforDetail p{
    margin-top: 10px;
  }
  .inforDetail p i{
    margin-right:10px; 
  }
  img{
    border:3px solid #8DEEEE;
    -moz-border-radius: 10px;
    -webkit-border-radius: 10px;
    border-radius: 10px;/*IE<9不支持*/
    position: absolute;
    top: 3px;
    right: 5%;
    height: 130px;
  }
  @media screen and (max-width:980px){
    img{
      display: none;
    }
    .inforWho{
      width: 40%;
    }
    .inforDetail{
      width: 49%;
      margin-left: 2%;
    }
  }
  @media screen and (max-width:680px){
    .inforWho,.inforDetail{
      display: block;
    }
    .inforWho{
      width: auto;
    }
    .inforDetail{
      width: auto;
      padding-left: 10px;
    }

  }
  @media screen and (max-width:450px){
    .name{
      font-size: 28px;
    }
    .job{
      font-size: 20px;
    }
    .inforDetail{
      font-size: 16px;
    }
  }
</style>
