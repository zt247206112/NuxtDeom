<template>
  <div>
      <h2>News Index page</h2>
      <p>NewsID：{{$route.params.newsId}}</p>
      <ul>
          <li>
              <nuxt-link :to="{name: 'index'}">HOME</nuxt-link>
          </li>
          <li>
              <nuxt-link :to="{name: 'news-id', params: {id: 123}}">news-1</nuxt-link>
          </li>
          <li>
              <nuxt-link :to="{name: 'news-id', params: {id: 456}}">news-2</nuxt-link>
          </li>
      </ul>
  </div>
</template>

<script>
export default {
    transition: 'test'
}
</script>

<style>

</style>