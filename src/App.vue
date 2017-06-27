<template>
  <div>
    <v-header></v-header>
    <div class="tab border-1px">
      <div class="tab-item">
        <a>商品</a>
      </div>
      <div class="tab-item">
        <a>评论</a>
      </div>
      <div class="tab-item">
        <a>商家</a>
      </div>
    </div>
    <v-shop></v-shop>
    <v-footer>huiihih</v-footer>
  </div>
</template>

<script>
import header from './components/header/header.vue';
import shop from './components/shop/shop.vue';
import footer from './components/footer/footer.vue';
export default {
  components: {
    'v-header': header,
    'v-shop': shop,
    'v-footer': footer
  }
};
window.addEventListener('orientationchange', setRem);
window.addEventListener('resize', setRem);
setRem();
function setRem() {
  var html = document.querySelector('html');
  var width = html.getBoundingClientRect().width;
  html.style.fontSize = width / 15 + 'px';
}
</script>

<style>
@import "index/css/reset.css";
@import "index/css/page.css";
</style>
