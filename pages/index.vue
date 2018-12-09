<template>
  <div>
    <div class='timg'>
      <img src="~static/timg.jpg" alt="">
    </div>
    <ul>
      <!-- <li><a href="/">home</a></li>
      <li><a href="/about">about</a></li>
      <li><a href="/news">news</a></li> -->
      <li><nuxt-link :to="{name:'index'}">home</nuxt-link></li>
      <li><nuxt-link :to="{name:'about'}">about</nuxt-link></li>
      <li><nuxt-link :to="{name:'news',params:{newsId: 123}}">news</nuxt-link></li>
      <li><nuxt-link :to="{name:'asyncData'}">asyncData</nuxt-link></li>
    </ul>
  </div>
</template>

<script>
// import AppLogo from '~/components/AppLogo.vue'

export default {
  components: {
    // AppLogo
  }
}
</script>

<style>
  .timg{
    width: 300px;
    height: 200px;
    background-image: url('~static/bg.png');
  }
  .timg img{
    height: 200px;
  }
</style>

