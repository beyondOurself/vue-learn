<template>
  <div :class="classes">
    <div class="navigates">
      <ul>
        <li>
          <h2>动态路由匹配</h2>
          <router-link to="/state">state</router-link>
          <router-link to="/getter">getter</router-link>
        </li>
      </ul>
    </div>
    <div class="show">
      <div class="show-content-wrap">
        <!-- 路由出口 -->
        <!-- 路由匹配到的组件将渲染在这里 -->
        <router-view></router-view>
        <!-- 命名视图 -->
      </div>
    </div>
  </div>
</template>
<script>
const prefixCls = "home";
export default {
  methods: {
  },
  computed: {
    classes() {
      return [`${prefixCls}`];
    }
  }
};
</script>
<style></style>
