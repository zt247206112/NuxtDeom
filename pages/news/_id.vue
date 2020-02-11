<template>
  <div>
      <h2>News-content</h2>
      <p>NewsId：{{$route.params.id}}</p>
      <ul>
          <li>
              <nuxt-link :to="{name: 'index'}">HOME</nuxt-link>
          </li>
      </ul>
  </div>
</template>

<script>
export default {
    validate({params}) {
        // 路由参数校验
        return /^\d+$/.test(params.id)
    }
}
</script>

<style>

</style>