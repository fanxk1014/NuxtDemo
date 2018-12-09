<template>
  <div>
    <ul>
      <!-- <li><a href="/">home</a></li>
      <li><a href="/about">about</a></li>
      <li><a href="/news">news</a></li> -->
      <li><nuxt-link :to="{name:'index'}">home</nuxt-link></li>
      <li><nuxt-link :to="{name:'about'}">about</nuxt-link></li>
      <li><nuxt-link :to="{name:'news',params:{newsId: 123}}">news</nuxt-link></li>
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

</style>

