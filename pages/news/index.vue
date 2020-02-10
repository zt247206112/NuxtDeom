<template>
  <div>
      <h2>News Index page</h2>
      <p>NewsID：{{$route.params.newsId}}</p>
      <ul>
          <li>
              <a href="/">HOME</a>
          </li>
          <li>
              <a href="/news/123">news-1</a>
          </li>
          <li>
              <a href="/news/456">news-2</a>
          </li>
      </ul>
  </div>
</template>

<script>
export default {
}
</script>

<style>

</style>