<template>
  <KView
    id="app"
    class="container">
    <router-link
      :to="routes.index"
      class="homeIcon">返回首页</router-link>
    <router-view/>
  </KView>
</template>

<script>
import Vue from 'vue'
import routes from '@/router/routeConfig'

export default Vue.extend({
    data() {
        return {
            routes
        }
    }
})
</script>
<style lang="less">
@import "./example.less";

.homeIcon{
    position: absolute;
    z-index: 2;
}
</style>
