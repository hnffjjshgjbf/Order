<template>
  <div class="footer">
    <div class="shopcart">
      <div class="content">
        <div class="content-left">
          <div class="logo-wrapper">
            <div class="logo">
              <i class="icon-shopping_cart"></i>
            </div>
            <!--<div class="num"></div>-->
          </div>
          <div class="price" :class="{'highlight':totalPrice>0}">￥0</div>
          <div class="desc">另需配送费￥4元</div>
        </div>
        <div class="content-right">
          <div class="pay">
            ￥20元起送
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {

  };
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style >

</style>
