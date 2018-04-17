<template>
  <div id='content2' class="">
    <div class="content2 container">
      <div class="div-box text col-lg-7 col-md-7 col-sm-7">
        <div>
          <p class="p1">Analyze & Learn their interest on your store</p>
          <p class="p2">By analyzing and learning their interests, Beeketing puts you a step ahead of the customer journey to predict products they're most likely to buy.</p>
          <img class="vector" src="./images/vector2.png" alt="vector">
        </div>
      </div>
      <div class="div-box img col-lg-5 col-md-5 col-sm-5">
        <img class="tablet" src="./images/tablet2.png" alt="tablet2">
      </div>
    </div>

    <!-- end content2 -->
  </div>
</template>

<script>
  export default {
    data () {
      return {
      }
    }
  }
</script>

<style lang="scss">
  //format conten2
  #content2{
    width:100%;
    @media only screen and (min-width: 1440px){
    .text{
      margin-top: 20%;
      .p1{
        font-size:30px;
      }
      .p2{
        color: #5b5b5b;
        font-size:22px;
      } 
    }
    .div-box{
      .vector{
        right: -100px;
        top: -20px;
        width: 144px;
        position: absolute;
      }
      .tablet{
        width: 90%;
        float: right;
        margin:70px 0px;
      }
    }
  }
  @media only screen and (max-width: 1439px){
  .text{
    margin-top: 20%;
    .p1{
      font-size:27px;
    }
    .p2{
      color: #5b5b5b;
      font-size:17px;
    } 
  }
  .div-box{
    .vector{
      right: -113px;
      top: -23px;
      width: 169px;
      position: absolute;
    }
    .tablet{
      width: 90%;
      float: right;
      margin:60px 0px;
    }
  }
}
@media only screen and (max-width: 1022px){
.text{
  margin-top: 19%;
  .p1{
    font-size:22px;
  }
  .p2{
    color: #5b5b5b;
    font-size:14px;
  } 
}
.div-box{
  .vector{
    right: -86px;
    top: -10px;
    width: 100px;
  }
      .tablet{
      width: 90%;
      margin:50px 0px;
    }
}
}
@media only screen and (max-width: 767px){
.text{
  margin-top: 30px;
  text-align: left;
  .p1{
    font-size:20px;
  }
  .p2{
    font-size:14px;
    text-align: left;
  } 
}
.div-box{
  .vector{
    display: none;
  }
      .tablet{
        float: none;
      width: 50%;
      display: block;
      margin: 0 auto;
    }
}
}
@media only screen and (max-width: 479px){
  .container{
    padding-left:0px;
    padding-right:0px;
  }
.text{
  margin-top: 30px;
  text-align: left;
  .p1{
    font-size:16px;
  }
  .p2{
    font-size:14px;
  } 
}
.div-box{
  .vector{
    display: none;
  }
      .tablet{
        float: none;
      width: 60%;
      display: block;
      margin: 0 auto;
      margin-bottom:30px;
    }
}
}
}

//end format content2
</style>
