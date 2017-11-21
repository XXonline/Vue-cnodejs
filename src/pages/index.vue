<template>
  <div class="item-box">
    <h1>{{ msg }}</h1>
  </div>
</template>

<script>
  export default {
    name: 'hello',
    data () {
      return {
        msg: 'sdfgs'
      }
    }
  }
</script>

<style scoped lang="less">
  @import "../assets/less/core/index.less";
</style>
