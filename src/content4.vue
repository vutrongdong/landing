<template>
  <div id="content4">

    <div class="moreapp">
      <h3>Ready to Get Started?</h3><br>
      <a>VIEW MORE APPS</a>
    </div>
    <hr>
    <!-- /////////////////// -->
    <div class="content4 container">
      <div id="carousel-id-4" class="carousel slide" data-ride="carousel">
        <ol class="carousel-indicators">
          <li data-target="#carousel-id-4" data-slide-to="0" class=""></li>
          <li  data-target="#carousel-id-4" data-slide-to="1" class=""></li>
          <li data-target="#carousel-id-4" data-slide-to="2" class="active"></li>
        </ol>
        <div class="carousel-inner">
         <!-- content1 -->
         <div class="item active">
          <div class="container">
            <div class="content4-1">
              <h3>E-marketing apps that give every sellers <b>the POWER</b><br> to sell sefectively like Amazon</h3><br><br>
              <img alt="Second slide" src="./images/slide-bottom-2.png">
              <p><i>"Beeketing has increase our conversion  rate by 23% and bring back the lost revenue within just a couple of weeks. The extra sales has paid for the app itseft for the whoie year!
                Definitely recommended!"</i></p>
                <h3 style="color:#006ae2;"> Helen jones</h3>
                <h4>FOUNDER AVIVA BOUTIQUE</h4><br><br>
                <div class="text">
                </div>
              </div>
            </div>
          </div> 
          <!-- end content1 -->

          <!-- //////conten2 -->
          <div class="item">
           <div class="container">
            <div class="content4-2">
              <div class="avt1 row">
                <div class="img col-lg-3 col-md-2 col-sm-2">
                  <img class="" alt="First slide" src="./images/avt1.png">
                </div>
                <div class=" text col-lg-9 col-md-10 col-sm-10 col-xs-12">
                  <img  src="./images/5sao.png" alt="5sao">
                  <h4 class="strong">really like this app. </h4>
                  <p>
                    The pop up is very attracrive. The customization was very easy. I enjoyed.
                    I enjoyed adding this to my shop. It made me feel like a big shot web store.
                    I got lots of good feedback form my friend who had been on the site several 
                    times throughout the set up process.
                  </p>
                </div>
              </div>
              <br>
              <hr>
              <div class="avt2 row">
                <div class="img col-lg-3 col-md-2 col-sm-2">
                  <img  class="" src="./images/avt2.png" alt="avt2">
                </div>
                <div class=" text col-lg-9 col-md-10 col-sm-10 col-xs-12">
                  <img src="./images/5sao.png" alt="avt2">
                  <h4 class="strong">Off Newbury</h4>
                  <p>
                    Super easy to use, love that it can be customized to match my store's color. Highly recommend this app!
                  </p>
                </div>
              </div>
              <hr>
              <div class="avt3 row">
                <div class="img col-lg-3 col-md-2 col-sm-2">
                  <img  class="" src="./images/avt3.png" alt="avt3">
                </div>
                <div class=" text col-lg-9 col-md-10 col-sm-10 col-xs-12" style="margin-bottom:70px;">
                  <img src="./images/3sao.png" alt="3sao"><h4 class="strong">Dronecyclone</h4>
                  <p >The app is solid and works well. However, it lacks any style control over the popup box. They do provide thems, but are mostly worthless. One size does not fit all. It is unfortunate that they have not provided full css
                    control and even access to their template code, as this would move it form a 3 star to a 5 star app.<br>
                    They should add an email field, linked to a mailchimp account. The idea being that each time a customer wants a discount
                    thet have to give the merchant something - brilliant idea, but missing critical pieces. This means you still have to use an email popup too.<br> But it does work, appears to be rock solid. It is producirg social likes so we are happy, just not as happy as if it did the above critical things. We would even be willing to pay a monthly fee for it, if it did the above. It just means we will have to keep looking for the perfect solution. Evolve or die. </p>

                  </div>
                </div>
              </div>
<!--                   <div class="logo-bottom" v-for="urls in url">
                    <div class="col-md-3 col-sm-6 col-xs-12"><a v-bind:href="urls.url_shop"><img v-bind:src="urls.src_img" alt=""></a></div>
                  </div>
                  <p ><a href="#" style="font-size:22px;margin-top:100px;">... and more</a></p>
                </div>
                <hr> -->
                <!-- end -->
              </div>
            </div>
          </div>
          <a style="; color: black;" class="left carousel-control" href="#carousel-id-4" data-slide="prev"><span class="glyphicon glyphicon-chevron-left"></span></a>
          <a style="; color: black;"  class="right carousel-control" href="#carousel-id-4" data-slide="next"><span class="glyphicon glyphicon-chevron-right"></span></a>
        </div>
      </div>
    </div>
  </div>
</div>
</template>

<script>
  export default {
    data () {
      return {
        show:false,
        url:[
        {src_img:"src/images/shop1.png",url_shop:"https://www.shopify.com"},
        {src_img:"src/images/shop2.png",url_shop:"https://github.com/SEOshop"},
        {src_img:"src/images/shop3.png",url_shop:"https://www.weebly.com"},
        {src_img:"src/images/shop4.png",url_shop:"https://tictail.com"},
        {src_img:"src/images/shop5.png",url_shop:"https://www.bigcommerce.com"},
        {src_img:"src/images/shop6.png",url_shop:"https://woocommerce.com"},
        {src_img:"src/images/shop7.png",url_shop:"https://magento.com"},
        {src_img:"src/images/shop8.png",url_shop:"https://beeketing.com"},
        ]
              // url:['https://www.shopify.com/','https://github.com/SEOshop','https://www.weebly.com/','https://tictail.com/','https://www.bigcommerce.com/','https://woocommerce.com/','https://magento.com/','https://beeketing.com/']
            };
          },
          methods:{
            show_app:function() {
              return 
              {
                show:this.show;
              }
            }
          }
        }
      </script>

      <style lang="scss">
        @mixin border-radius($border-radius){
        -webkit-border-radius:$border-radius;
        -moz-border-radius: $border-radius;
        -mst-border-radius: $border-radius;
        -o-border-radius: $border-radius;
        border-radius: $border-radius;
      }
      /////////////////////
      #content4{
        @mixin border-radius($border-radius){
        -moz-border-radius: $border-radius;
        -ms-border-radius: $border-radius;
        border-radius: $border-radius;
      }
      .moreapp{
        text-align: center;
      }
      #carousel-id-4{
        //border: 1px solid blue;
        .left,.right{
          background: none;
        }
        ol{
          li{
            width: 20px;
            height: 20px;
            background: #d9d9d9;
          }
          .active{
            background: #006ae2;
          }
        }
      }
      @media screen and (min-width: 1440px){
      .moreapp{
        margin-bottom: 40px;
        h3{
          font-size: 30px
        }
        a{
          padding: 20px 10px;
          color: #fff;
          background: #12ca64;
          @include border-radius(7px);
          &:hover{
            background: #1fd771;
            text-decoration: none;
          }
        }
      }
      // end moreapp//

      // carousel-id-4 //

      #carousel-id-4{
        ol{
          margin-top: 30px;
          li{
            width: 20px;
            height: 20px;
          }
        }
        .carousel-inner{
          .item{
            text-align: center;
            // begin conten4-1
            .content4-1{
             margin: 90px 0px 82px 0px;
             h3{
              color: #383838;
              font-size:30px;
            }
            img{
              margin: 100px 0px;
            }
            p{
              font-size: 18px;
              color: #5b5b5b;
              width: 65%;
              margin: 0 auto;
              display: block;
            }
          }
          // end content4-1

          // begin content4-2
          .content4-2{
            width: 90%;
            margin: 0 auto;
            display: block;
            text-align: left;
            .row{
              .img{
                img{
                  margin: 0 auto;
                  display: block;
                }
              }
            }
            .text{
              h4{
                margin-top: 0px; 
                margin-bottom: 20px;
                font-size: 20px;
              }
              p{
                font-size: 16px;
                color: #5b5b5b;
                padding-right: 50px;
              }
            }
          }
          // end conten4.2
        }
      }
    }
    // /end carousel-id-4
  }
}
@media screen and (max-width: 1440px){
.moreapp{
  margin-bottom: 40px;
  h3{
    font-size: 30px
  }
  a{
    padding: 17px 9px;
    color: #fff;
    background: #12ca64;
    @include border-radius(7px);
    &:hover{
      background: #1fd771;
      text-decoration: none;
    }
  }
}
// end moreapp//

// carousel-id-4 //

#carousel-id-4{
  ol{
    margin-top: 27px;
    li{
      width: 20px;
      height: 20px;
    }
  }
  .carousel-inner{
    .item{
      text-align: center;
      // begin conten4-1
      .content4-1{
       margin: 104px 0px 100px 0px;
       h3{
        color: #383838;
        font-size:25px;
      }
      img{
        margin: 70px 0px;
      }
      p{
        font-size: 16px;
        color: #5b5b5b;
        width: 65%;
        margin: 0 auto;
        display: block;
      }
    }
    // end content4-1

    // begin content4-2
    .content4-2{
      width: 85%;
      margin: 0 auto;
      display: block;
      text-align: left;
      .row{
        .img{
          img{
            width: 90%;
            margin: 0 auto;
            display: block;
          }
        }
      }
      .text{
        h4{
          margin-top: 0px; 
          margin-bottom: 20px;
          font-size: 18px;
        }
        p{
          font-size: 15px;
          color: #5b5b5b;
          padding-right: 50px;
        }
      }
    }
    // end conten4.2
  }
}
}
// /end carousel-id-4
@media screen and (max-width: 1023px){
.moreapp{
  margin-bottom: 40px;
  h3{
    font-size: 25px
  }
  a{
    padding: 15px 8px;
    @include border-radius(7px);
  }
}
// end moreapp//

// carousel-id-4 //

#carousel-id-4{
  ol{
    margin-top: 20px;
    li{
      width: 20px;
      height: 20px;
    }
  }
  .carousel-inner{
    .item{
      // begin conten4-1
      .content4-1{
       margin: 80px 0px 80px 0px;
       h3{
        font-size:20px;
      }
      img{
        margin: 50px 0px;
      }
      p{
        font-size: 15px;
        width: 65%;
      }
    }
    // end content4-1

    // begin content4-2
    .content4-2{
      width: 80%;
      .row{
        .img{
          img{
            width: 90%;
          }
        }
      }
      .text{
        img{
          width:10%;
        }
        h4{
          margin-top: 0px; 
          margin-bottom: 10px;
          font-size: 15px;
        }
        p{
          font-size: 14px;
          color: #5b5b5b;
          padding-right: 20px;
        }
      }
    }
    // end conten4.2
  }
}
}
// /end carousel-id-4
}
@media screen and (max-width: 768px){
.container{
  padding-left:0px;
  padding-right:0px;
}
.moreapp{
  margin-bottom: 40px;
  h3{
    font-size: 22px
  }
  a{
    padding: 12px 6px;
    @include border-radius(5px);
  }
}
// end moreapp//

// carousel-id-4 //

#carousel-id-4{
  hr{
    margin-top: 0px;
    margin-bottom: 0px;
  }
  .left,.right{
    font-size: 10px;
  }
  ol{
    margin-top: 20px;
    li{
      width: 20px;
      height: 20px;
    }
  }
  .carousel-inner{
    .item{
      // begin conten4-1
      .content4-1{
       margin: 80px 0px 80px 0px;
       h3{
        font-size:15px;
        padding: 0px 10px;
      }
      img{
        width: 200px;
        margin: 40px 0px;
      }
      p{
        font-size: 15px;
        width: 65%;
      }
      h4{
        font-size:14px;
      }
    }
    // end content4-1

    // begin content4-2
    .content4-2{
      width: 80%;
      .row{
        .img{
          display: none;
        }
      }
      .text{
        margin-top:5px;
        img{
          width:50px;
        }
        h4{
          margin-top: 0px; 
          margin-bottom: 10px;
          font-size: 14px;
        }
        p{
          font-size: 13px;
          padding-right: 0px;
        }
      }
    }
    // end conten4.2
  }
}
}
// /end carousel-id-4
}
}
</style>
