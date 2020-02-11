<template>
  <div>
    <div class="diss">
    </div>
    <ul>
      <li>
        <nuxt-link :to="{name: 'index'}">HOME</nuxt-link>
      </li>
      <li>
        <nuxt-link :to="{name: 'about'}">ABOUT</nuxt-link>
      </li>
      <li>
        <nuxt-link :to="{name: 'news', params: {newsId: 3306}}">NEWS</nuxt-link>
      </li>
      <li>
        <nuxt-link :to="{name: 'asyncData'}">asyncData</nuxt-link>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  components: {}
}
</script>

<style>
  .diss {
    width: 982px;
    height: 55px;
    background: url('~static/logo.png') no-repeat;
  }
</style>