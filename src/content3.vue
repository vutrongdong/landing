<template>
  <div id='content3'>
    <!-- begin content3 -->
    <div class="content3 container">
      <div class="text">
        <p class="p1">Smart Marketing Apps to turn your visitors into revenue<p>
          <p class="p2">From the da ta collected, we buld a platform of smart marketing apps to follow your visitors right when they step on your store
            and gradually convert them to customers - then loyal custorners for you</p>
          </div>
          <!-- begin laptop -->
          <div class="laptop">
            <div id="carousel-id" class="carousel slide" data-ride="carousel">
              <div class="carousel-inner">
                <div class="item">
                  <img alt="1" src="./images/screen1.png">
                </div>
                <div class="item">
                  <img  alt="2" src="./images/screen2.png">
                </div>
                <div class="item">
                  <img  alt="3" src="./images/screen3.png">
                </div>
                <div class="item">
                  <img  alt="4" src="./images/screen4.png">
                </div>
                <div class="item active">
                  <img  alt="5" src="./images/screen5.png">
                </div>
              </div>
            </div>
          </div>
          <!-- end laptop -->
          <!-- begin carousel3d -->
          <div class="carousel-3d" >
           <carousel-3d height="490px">
            <slide v-for="(slide, i) in carousel3d" v-bind:index="i" style="opacity: 0.5">
              <img :src="slide.img" alt="">
              <h2 :class="slide.class">{{slide.title}}</h2>
              <h3 :class="slide.class">{{slide.content}}</h3>
              <button>Learn more</button>
            </slide>
          </carousel-3d>
        </div>
        <!-- end carousel 3d -->
      </div>
      <!-- end content3 -->
    </div>
  </template>

  <script>
   import {Carousel3d, Slide } from 'vue-carousel-3d';
   export default {
    components:{Carousel3d, Slide},
    data () {
      return {
        carousel3d:[
        {class:"coupon",img:"src/images/object1.png",title:"Better Coupon Box",content:"Popup a coupon box to turn visitors into social followers, email subscribers and increase your sales"},
        {class:"product",img:"src/images/object3.png",title:"Product Recommendation",content:"Target Recommendations to the right customers around their shoppong jourrey on your store."},
        {class:"email",img:"src/images/object2.png",title:"Email automation",content:"Follow up your customers with automated emails personnalized to their behaviors"}
        ],
      }
    }
  }
</script>

<style lang="scss">
  #content3{
    @mixin border-radius($border-radius){
    -moz-border-radius: $border-radius;
    -ms-border-radius: $border-radius;
    border-radius: $border-radius;
  }
  background: #ececec;
  text-align: center;
  .laptop{
    background-image: url("./images/mac.png");
    background-size: 100%;
    background-repeat: no-repeat;
  }
  // format carousel3d
  .carousel-3d-container{
    .carousel-3d-slider{
      border: none;
      .carousel-3d-slide{
        opacity: 0.5;
        background: none;
        border: none;
        h2,h3,button{
          position: absolute;
        }
        h2{
          top: 120px;
          text-align: center;
          font-size: 30px;
        }
        h3{
          font-size: 20px;
          top: 180px;
          text-align: center;
          padding: 0px 15px;
          color: #5b5b5b;
        }
        h2.coupon{
          left:53px;
        }
        h3.product{
          top: 210px;
        }
        h2.product{
          left:40px;
          right: 40px;
        }
        h2.email{
          left: 65px;

        }
        button{
          background:#2b9cff;
          padding: 20px 60px;
          color: #fff;
          top: 327px;
          left:45px;
          font-size:27px;
          @include border-radius(7px);
        }
        img{

        }
      }
    }
  }
  //end carousel3d
  @media only screen and (min-width:1023px)
  {
  .text{
    margin-top: 40px;
    .p1{
      font-size:30px;
    }
    .p2{
      color: #5b5b5b;
      font-size:20px;
    }
  }
  .laptop{
    width:863px;
    height:500px;
    margin: 0 auto;
    margin-top:30px;
    padding-left: 116px;
    padding-right:110px;
    #carousel-id{
      .carousel-inner{
        bottom:-44px;
        img{
          margin:0 auto;
        }
      }
    }
  }
}

@media only screen and (max-width:1022px)
{
 .text{
  margin-top: 40px;
  .p1{
    font-size:25px;
  }
  .p2{
    color: #5b5b5b;
    font-size:16px;
  }
}
.laptop{
  width:600px;
  height:400px;
  margin: 0 auto;
  margin-top:30px;
  padding-left: 107px;
  padding-right:103px;
  #carousel-id{
    .carousel-inner{
      bottom:-30px;
      img{
        margin:0 auto;
      }
    }
  }
}
}

@media only screen and (max-width:767px)
{
  .text{
    padding-left: 15px;
    text-align:left;
    margin-top: 40px;
    .p1{
      font-size:20px;
    }
    .p2{
      color: #5b5b5b;
      font-size:14px;
    }
  }
  .laptop{
    width:450px;
    height:350px;
    margin-top:30px;
    padding-left: 76px;
    padding-right:76px;
    #carousel-id{
      .carousel-inner{
        bottom:-21px;
      }
    }
  }
  // format carousel3d
  .carousel-3d-container{
    .carousel-3d-slider{
      border: none;
      .carousel-3d-slide{
        text-align:center;
        opacity: 0.5;
        background: none;
        border: none;
        h2,h3,button{
          position: absolute;
        }
        h2{
          top: 120px;
          text-align: center;
          font-size: 20px;
        }
        h3{
          font-size: 15px;
          top: 180px;
          text-align: center;
          padding: 0px 50px;
          color: #5b5b5b;
        }
        h2.coupon{
          left:95px;
        }
        h3.product{
          top: 210px;
        }
        h2.product{
          left:40px;
          right: 40px;
        }
        h2.email{
          left: 100px;

        }
        button{
          background:#2b9cff;
          padding: 10px 30px;
          color: #fff;
          top: 327px;
          left:96px;
          font-size:20px;
          @include border-radius(7px);
        }
        img{
          float: none;
          width: 300px;
        }
      }
    }
  }
  //end carousel3d
}
@media only screen and (max-width:479px)
{
  .container{
    padding-left: 0px;
  }
  .text{
    padding-left:15px;
    margin-top: 40px;
    .p1{
      font-size:18px;
    }
    .p2{
      text-align: left;
      color: #5b5b5b;
      font-size:13px;
    }
  }
  .laptop{
    width:250px;
    height:200px;
    margin-top:20px;
    padding-left: 43px;
    padding-right:43px;
    #carousel-id{
      .carousel-inner{
        bottom:-12px;
      }
    }
  }
  // format carousel3d
  .carousel-3d-container{
    display: none;
  }
  //end carousel3d
}
}
</style>
