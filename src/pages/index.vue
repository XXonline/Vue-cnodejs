<template>
  <div class="item-box">
    <mu-date-picker></mu-date-picker>
    <mu-drawer></mu-drawer>
  </div>
</template>

<script>
  import http from '../utils/http'
  import api from '../utils/api'

  export default {
    name: 'hello',
    data () {
      return {}
    },
    mounted: function () {
      this.fetchData()
    },
    methods: {
      fetchData: async function () {
        let params = {}
        const res = await http.get(api.right, params)
        if (res.data.success) {
          alert('请求成功')
          console.log('res:', res.data)
        }
      }
    }
  }
</script>

<style scoped lang="less">
  @import "../assets/less/core/index.less";
</style>
