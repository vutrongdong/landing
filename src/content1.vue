<template>
  <div id="content1">
    <div class="content1 container">
      <div class="text ">
        <h2 class="margin-center">{{h2}}</h2>
        <p class="play-video margin-center p-color">{{play_video}}<img v-on:click="show=!show" src="./images/icon-video.png" alt="icon-video"></p>
        <video v-show="show" width="100%" controls>
          <source src="http://www.w3schools.com/html/mov_bbb.mp4" type="video/mp4">
          </video>
        </div>
        <div class="tablet1">
          <div class="div-box col-lg-6 col-md-6 col-sm-6">
            <img style="vertical-align: middle;"  class="tablet" src="./images/tablet1.png"  alt="tablet1">
            <img  class="vector" src="./images/vector1.png"  alt="vector">
          </div>
          <div class="text col-lg-6 col-md-6 col-sm-6">
            <p class="p1">{{p1}}</p>
            <p class="p2">{{p2}}</p>
          </div>
        </div>
      </div>
    </div>
  </template>

  <script>
    export default {
      data () {
        return {
          h2:"How it works",
          play_video:"PLAY VIDEO INTRO",
          p1:"Track your customers' behaviors",
          p2:"every visit to your store gets tied to a real person. Beeketing helps you see who they are, know what they do on your store",
          show:false
        }
      },
      methods:{
        show_video:function(){
         return {
          show:this.show
        };
      }
    }
  }
</script>

<style lang="scss">
  body{
    max-width:1900px;
    margin: 0 auto;
  }
  #content1{
    background: #ececec;}
    .p-color {
      color: #108ffe;
    }
    .margin-center{
      text-align:center;
    }
    @media only screen and (min-width: 1440px){
    .content1{
      h2{
        padding-top:40px;
        font-size: 50px;
      }
      .tablet1{
        margin-top:50px;
        .p1{
          font-size:30px;
          color:#141010;
        }
        .p2{
          color: #5b5b5b;
          font-size:20px;
        }
        .tablet{
          width: 90%;
        }
        .vector{
          position: absolute;
          top: 80px;
          right: 0;
        }
        .text{
          margin-top: 5%;
        }
      }
    }
  }
  @media only screen and (max-width: 1439px){
  .content1{
    h2{
      padding-top:40px;
      font-size: 45px;
    }
    .play-video{
      font-size: 18px;
    }
    .tablet1{
      margin-top:50px;
      .p1{
        font-size:27px;
        color:#141010;
      }
      .p2{
        font-size:17px;
        color: #5b5b5b;
      }
      .tablet{
        width: 90%;
      }
      .vector{
        position: absolute;
        top: 140px;
        width: 23%;
        right: 0;
      }
      .text{
        margin-top: 12%;
      }
    }
  }
}
@media only screen and (max-width: 1022px){
.content1{
  h2{
    padding-top:40px;
    font-size: 35px;
  }
      .play-video{
      font-size: 16px;
      img{
        width: 30px;
      }
    }
  .tablet1{
    margin-top:50px;
    .p1{
      font-size:22px;
      color:#141010;
    }
    .p2{
      font-size:14px;
      color: #5b5b5b;
    }
    .tablet{
      width: 90%;
    }
    .vector{
      position: absolute;
      top: 80px;
      width: 25%;
      right: 0;
    }
    .text{
      margin-top: 7%;
    }
  }
}
}
@media only screen and (max-width: 768px){
.content1{
  h2{
    padding-top:40px;
    font-size: 27px;
  }
      .play-video{
      font-size: 12px;
            img{
        width: 25px;
      }
    }
  .tablet1{
    margin-top:20px;
    .p1{
      font-size:18px;
      color:#141010;
    }
    .p2{
      font-size:14px;
      color: #5b5b5b;
    }
    .tablet{
      width: 60%;
      margin: 0 auto;
      display: block;
    }
    .vector{
     display:none;
    }
    .text{
      text-align: left;
      margin-top: 3%;
      margin-bottom:20px;
    }
  }
}
}
@media only screen and (max-width: 479px){
  h2{
    font-size:25px;
  }
  #content1{
  .container{
    padding-left: 0px;
    padding-right: 0px;
  }
}
        .play-video{
      font-size: 12px;
            img{
        width: 20px;
      }
    }
  .tablet1{
    text-align:left;
    .p1{
      font-size:16px;
      color:#141010;
    }
    .p2{
      font-size:14px;
    }
    img{
      margin: 0 auto;
      display:block;
    }
  }
  .text{
    margin-top:20px;
  }
}


//end format content1
</style>
