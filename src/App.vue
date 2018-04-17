<template>
  <div id="app">
    <bannertop></bannertop>
    <content1></content1>
    <content2></content2>
    <content3></content3>
    <content4></content4>
    <appfooter></appfooter>
  </div>
</template>

<script>
 import banner_top from './bannertop.vue';
 import content1 from './content1.vue';
import content2 from './content2.vue';
import content3 from './content3.vue';
import content4 from './content4.vue';
import footer from './footer.vue';
export default {
  components:{
    'bannertop':banner_top,
    'content1' :content1,
    'content2' :content2,
     'content3' :content3,
      'content4' :content4,
      'appfooter':footer
  },
  data () {
    return {
      
    }
  }
}
</script>

<style lang="scss">
  html,body{
    font-family: arial , arial black, sans serif, serif,display,scrip;
    color: black;
  }
  *{
  margin:0px;
  padding:0px;
}
</style>
