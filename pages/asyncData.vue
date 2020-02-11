<template>
  <div>
      <h1>姓名：{{info.name}}</h1>
      <h1>年龄：{{info.age}}</h1>
      <h1>兴趣：{{info.interest}}</h1>
  </div>
</template>

<script>
import axios from 'axios'
export default {
    data () {
        return {
            name: 'Hello World'
        }
    },
    methods: { },
    // nuxt默认的方法
    // asyncData () {
    //     return axios.get('https://api.myjson.com/bins/1gpdok')
    //     .then((res) => {
    //         return {
    //             info: res.data, // 相当于在data里加了个info属性
    //         }
    //     })
    // }
    // 两种方式，推荐async await
    async asyncData () {
        let { data } = await axios.get('https://api.myjson.com/bins/1gpdok');
        return {
            info: data
        }
    }
}
</script>

<style>

</style>