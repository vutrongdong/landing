<template>
  <div id='banner-top'>
    <!-- menu top -->
    <menutop></menutop>
    <!-- end menutop -->
    <div class="container">
      <div class="text inline col-lg-8 col-md-8 container" > 
        <h3 >Convert Customer</h3>
        <h1 >Personally  Automatically</h1>
        <h4 >Your customers all behave differentlly. Why treat them all the same?</h4>
        <a  class="btn btn-info" href="#">{{button}}</a>
        <img id="vector" src="./images/vector.png" >
        <!-- //////////////// slide-top1 -->
        <div id="carousel-id-text" class="carousel slide load" data-ride="carousel">
          <div class="carousel-inner">
            <div class="item">
              <img alt="First slide" src="./images/abc.png">
              <div class="container">
                <div class="carousel-caption">
                  <h3>Checkout Boost</h3>
                  <p>Boost revenue & sccial word</p>
                </div>
              </div>
            </div>
            <div class="item">
              <img alt="Second slide" src="./images/abc.png">
              <div class="container">
                <div class="carousel-caption">
                  <h3>Better Coupon Box</h3>
                  <p>Increase social followers & sales</p>
                </div>
              </div>
            </div>
            <div class="item active">
              <img  alt="Third slide" src="./images/abc.png">
              <div class="container">
                <div class="carousel-caption">
                  <h3>Boost Sales</h3>
                  <p>Up-sell & Cross-sell in 1 app </p> 
                </div>
              </div>
            </div>
          </div>
          <div class="carousel-left-right">
            <a class="left carousel-control" href=".load" data-slide="prev"><span class="glyphicon glyphicon-chevron-left"></span></a>
            <a class="right carousel-control" href=".load" data-slide="next"><span class="glyphicon glyphicon-chevron-right"></span></a>
          </div>
        </div>

        <!--  -->
        <!-- text & slide-show top -->
        <div class="slide-top">
          <p>Helping more than <strong>6.000 online sellers</strong> to sell to millions of customers</p>
          <div class="slide-show-top">
            <div id="carousel-id1"  class="carousel slide" data-ride="carousel">
              <div class="carousel-inner">
                <div class="item">
                  <img alt="First slide" width="40%" src="./images/slide-show-top.png">
                </div>
                <div class="item">
                  <img  alt="Second slide" width="40%" src="./images/slide-show-top.png">
                </div>
                <div class="item active">
                  <img  alt="Third slide" width="40%" src="./images/slide-show-top.png">
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>

      <!-- ///////////////////// end slidetop 1-->
      <div class="smartphone col-lg-4 col-md-4">
        <div id="carousel-id" class="carousel slide load" data-ride="carousel">
          <div class="carousel-inner">
            <div class="item">
              <img  alt="First slide" src="./images/display1.png">
            </div>
            <div class="item">
              <img alt="Second slide" src="./images/display2.png">
            </div>
            <div class="item">
              <img  alt="Second slide" src="./images/display3.png">
            </div>
            <div class="item">
              <img   alt="Second slide" src="./images/display4.png">
            </div>
            <div class="item">
              <img alt="Third slide" src="./images/display5.png">
            </div>
            <div class="item active">
              <img  alt="Second slide" src="./images/display6.png">
            </div>
          </div>      
        </div>
      </div>
      <div>
        <br>
      </div>
      <!-- text & slide-show top -->
    </div>

    <!-- /////////////////////////////////// -->
  </div>
</template>

<script>
 import menutop from './menu_top.vue';
 export default {
  components:{menutop},
  data () {
    return {
      button:"Get started now",
    }
  }
}
</script>

<style lang="scss">
  @mixin border-radius($border-radius){
  -moz-border-radius: $border-radius;
  -ms-border-radius: $border-radius;
  border-radius: $border-radius;
}
#banner-top{
  width:100%;
  color: #fff;
  background: no-repeat;
  clear:both;
  #carousel-id-text{
    clear: both;
    h3{
      color: #0088ff;
    }
  }
}
.submit{
  background:#0088ff;
  color: #fff;
  font-size:22px;
  &:hover{
    background:#8AE234;
    text-decoration: none;
    transition: all 1s 0.3s;
    color:black;
  }
}
.smartphone{
  background-image: url("images/iphone6.png");
  background-size: 100%;
  background-repeat: no-repeat;

}
.slide-top{ 
  clear:both;
  color:black;
  text-align: center;
  .slide-show-top{
    img{
      display: block;
      margin:0 auto;
    }
  }
  .left,.right{
    background:none;
    width:500px;
  }
}
@media only screen and (min-width: 1441px){
#banner-top{
  background-image: url("./images/banner-top.png");
  #carousel-id-text{
    margin-top:130px;
    float: right;
    width: 334px;
    .carousel-caption{
      bottom: -23px;
      h3{
        font-size: 14px;
      }
      p{
        font-size:13px;
      }
    }
  }
  .text{
    h3,h1,h4{
      margin:0;
      background:blue;

    }
    h4{
      font-size: 20px;
    }
    h3{
      margin-top: 90px;
      font-size: 40px;
    }
    h1{
      font-size: 60px;
      margin-bottom: 90px;
    }
    #vector{
      position: absolute;
      right:-27px;

    }
    .btn{
      padding: 10px 15px;
      background: #0088ff;
      margin-top:20px;
      font-size: 20px;
    }
  }
  .smartphone{
    width:330px;
    margin-top:80px;
    height:720px;
    float:right;
    padding-left:20px;
    padding-right:20px;
    #carousel-id{

      img{
        opacity: 0;
        display: block;
        margin: 0 auto;
        margin-top:70px;
      }
      .carousel-inner{
        .item {
          opacity:1;
          transition: opacity 1s 0.1s;
        }
        .active{
          img{
            opacity: 1;
          }
        }
        .left{
          opacity:    0;
        }
      }
    }

  }
  .slide-top{

    margin: 235px 0px 0px 0px;
    font-size:19px;
    img{
      width: 100%;
    }
  }
}
}
//format for screen 1023px;{}
@media only screen and (max-width: 1440px){
#banner-top{
  background-image: url("./images/banner-top.png");
  #carousel-id-text{
    margin-top:130px;
    float: right;
    width: 334px;
    .carousel-caption{
      bottom: -23px;
      h3{
        font-size: 14px;
      }
      p{
        font-size:13px;
      }
    }
  }
  .text{
    h3,h1,h4{
      margin:0;

    }
    h4{
      font-size: 16px;
    }
    h3{
      margin-top: 90px;
      font-size: 35px;
    }
    h1{
      font-size: 46px;
      margin-bottom: 90px;
    }
    #vector{
      position: absolute;
      right:-30px;

    }
    .btn{
      padding: 10px 15px;
      background: #0088ff;
      margin-top:20px;
      font-size: 20px;
    }
  }
  .smartphone{
    width:300px;
    margin-top:80px;
    height:680px;
    float:right;
    padding-left:20px;
    padding-right:20px;
    #carousel-id{
      img{
        display: block;
        margin: 0 auto;
        margin-top:70px;
      }
    }

  }
  .slide-top{
    font-size:17px;
    margin: 248px 0px 0px 0px;
    img{
      width: 100%;
    }
  }
}
}
// format for screen than less 1022px
//format for screen 1023px;{}
@media only screen and (max-width: 1023px){
#banner-top{
  .container{
    width: none;
  }
  text-align: center;
  background: #3355e7;
  #carousel-id-text{
    margin: 0 auto;
    margin-top:20px;
    margin-bottom: 15px;
    float: none;
    width: 334px;
    .carousel-caption{
      bottom: -23px;
      h3{
        font-size: 14px;
        color: red;
        text-shadow: none;
      }
      p{
        font-size:13px;
      }
    }
    .carousel-left-right{
      .left,.right{
        background: none;
      }
    }
  }
  .text{
    width: 100%;
    h3,h1,h4{
      margin:0;

    }
    h4{
      font-size: 15px;
    }
    h3{
      margin-top: 30px;
      font-size: 22px;
    }
    h1{
      font-size: 30px;
      margin-bottom: 20px;
    }
    #vector{
      display: none;
    }
      .btn{
    font-size:15px;
    padding:8px 10px;
    @include border-radius(5px);
  }
  }
  .smartphone{
    clear: both;
    width:300px;
    margin-top:20px;
    height:617px;
    float:none;
    margin: 0 auto;
    padding-left:20px;
    padding-right:20px;
    #carousel-id{
      img{
        display: block;
        margin: 0 auto;
        margin-top:70px;
      }
    }
  }
  .slide-top{
    display: none;
    margin: 20px 0px 0px 0px;
  }
}
}
@media only screen and (max-width: 767px){
#banner-top{
  #carousel-id-text{
    .carousel-caption{
        padding-bottom: 32px;
    }
  }
  .text{
    text-align:center;
    display: block;
    width:100%;
    padding-top: 20px;
    h4{
      font-size: 14px;
    }
    h3{
      margin-top: 22px;
      font-size: 18px;
    }
    h1{
      padding-top:10px;
      font-size: 25px;
      margin-bottom: 20px;
    }
      .btn{
    font-size:14px;
    padding:6px 8px;
    @include border-radius(5px);
  }
  }
  .slide-top{
    margin-top: 20px;
    margin-left:5%;
    text-align:center;
  }
  .smartphone{
    clear: both;
    display: block;
    padding-left:15px;
    padding-right:15px;
    margin-top:0px;
    width:250px;
    height:520px;
    #carousel-id{
      top: -10px;
      width:100%;
      img{
        width:100%;

      }
    }
  }
}
}

@media only screen and (max-width: 479px){
#banner-top{
   #carousel-id-text{
    display: none;
  }
  .text{
    width:100%;
    padding-top: 0px;
    h4{
      font-size: 13px;
    }
    h3{
      margin-top: 22px;
      font-size: 16px;
    }
    h1{
      padding-top:10px;
      font-size: 18px;
      margin-bottom: 10px;
    }
      .btn{
    padding:5px 8px;
    font-size:13px;
    @include border-radius(3px);
    top:20px;
  }
  }
  .smartphone{
    padding-left:19px;
    padding-right:19px;
    margin-top:20px;
    width:200px;
    height:400px;
  }
}
}
</style>
