<template>
  <div id="footer">
        <!-- begin bottom -->
        <div class="background-bottom">
          <div class="text">
            <p class="p1">READY TO INCREASE YOUR SALES BY 20%+ ?</p>
            <p class="p2"> No sales team, no marketers, no engineers. Just results & Beeketing.</p>
            <a class="get-started-now" v-bind:href="url">Get started now</a>
    
          </div>
          <div>
            <nav class="inline">
              <a href="#" v-for="element in menu_bottom">{{element}}</a>
            </nav>
            <img class="inline" src="./images/logo-bottom.png" alt="logo"><br>
            <p>Contact Us | Beeketing 2015.Al right reserved.</p>
          </div>

        </div>
        <!-- end bottom -->
      </div>
  </div>
</template>

<script>
  export default {
    data () {
      return {
          menu_bottom:["Blog","Prees kit","Careers","Contact"],
          url:"#"
      }
    }
  }
</script>

<style lang="scss">
#footer{
  clear:both;
    @mixin border-radius($border-radius){
  -webkit-border-radius:$border-radius;
  -moz-border-radius: $border-radius;
  -mst-border-radius: $border-radius;
  -o-border-radius: $border-radius;
  border-radius: $border-radius;
}
.background-bottom{
  .text{
    p{
      color: #fff;
    }
    .get-started-now{
      background: #fb1ca4;
      padding:2%;
      color: #fff;
      &:hover{
        background:#b2568e;
        text-decoration: none;
        color: #fff;
      }
    }
  }
  div{
    nav{
      margin-left: auto;
      margin-right:auto;
      a{
        color:#fff;
        font-weight: bold;
        &:hover{
          color:#0270d5;
          text-decoration: none;
        }
      }

    }
  }
}
@media screen and (min-width:1441px){
    .background-bottom{
  background-image: url("images/background-bottom.png");
  background-size: 100%;
  background-repeat: no-repeat;
  text-align: center;
  color: #fff;
}
    .text{
      padding-top:20%;
      .p1{
        font-size:35px;
      }
      .p2{
        font-size:22px;
        margin-bottom:100px;
      }
      a{
        @include border-radius(5px);
        font-size:20px;
      }
    }
    nav{
      background:#071130;
      width:400px;
      height: 40px;
      line-height: 40px;
      margin-top:15%;
      margin-bottom:10px;
      a{
        padding:0px 15px;
      }
      p{
        padding-bottom:20px;
      }

    }
}
  @media screen and (max-width: 1440px)
  {
  .background-bottom{
  background-image: url("images/background-bottom.png");
  background-size: 100%;
  background-repeat: no-repeat;
  text-align: center;
  color: #fff;
}
    .text{
      padding-top:12%;
      .p1{
        font-size:35px;
      }
      .p2{
        font-size:22px;
        margin-bottom:100px;
      }
      a{
        @include border-radius(5px);
        font-size:20px;
      }
    }
    nav{
      background:#071130;
      width:400px;
      height: 40px;
      line-height: 40px;
      margin-top:19%;
      a{
        padding:0px 15px;
      }

    }

  }
  @media screen and (max-width: 1022px)
  {
  .background-bottom{
  background:#003874;
  background-size: 100%;
  background-repeat: no-repeat;
  text-align: center;
  color: #fff;
}
    .text{
      padding-top:10%;
      .p1{
        font-size:23px;
      }
      .p2{
        font-size:21px;
        margin-bottom:50px;
      }
      a{
        @include border-radius(4px);
        font-size:17px;
      }
    }
    nav{
      width:70%;
      height: 40px;
      line-height: 40px;
      margin-top:5%;
      a{
        padding:0px 10px;
      }

    }
    img{
      width:250px;
      margin:10px 0px;
    }
    p{
      font-size:17px;
      padding-bottom:10px;
    }
  }
  @media screen and (max-width: 767px)
  {
    .text{
      padding-top:12%;
      .p1{
        font-size:20px;
      }
      .p2{
        font-size:17px;
        margin-bottom:40px;
      }
      a{
        @include border-radius(3px);
        font-size:17px;
      }
    }
    nav{
      width:80%;
      height: 40px;
      line-height: 40px;
      margin-top:10%;
      a{
        font-size:15px;
        padding:0px 15px;
      }

    }
    img{
      width:250px;
      margin: 10px 0px;
    }
    p{
      font-size:17px;
      padding-bottom:10px;
    }
  }
  @media screen and (max-width: 479px)
  {
    .text{
      padding-top:10%;
      .p1{
        font-size:13px;
      }
      .p2{
        font-size:12px;
        margin:0px 5px;
        margin-bottom:10px;
      }
      p{
        padding-bottom: 4px;
      }
      a{
        @include border-radius(2px);
      }
    }
    nav{
      background: none;
      width: none;
      height: 35px;
      line-height: 35px;
      margin-top:10%;
      a{
        font-size:12px;
        padding:0px 5px;
        &:hover{
          color: red;
        }
      }

    }
    img{
      width:200px;
      margin:10px 0px;
    }
    p{
      font-size:11px;
      padding-bottom:15px;
    }
  }
}
</style>
