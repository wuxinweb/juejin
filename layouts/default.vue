<template>
  <div>
    <!-- 头部组件 -->
    <Head :navs="navs"/>
    <!-- 路由 -->
    <nuxt/>
  </div>
</template>

<script>
import Head from "@/components/common/head/head";
import { mapState } from "vuex";
export default {
  mounted() {
    
  },
  components: {
    Head
  },
  computed: {
    ...mapState(["navs"])
  }
};
</script>

<style>
html,
body {
  background-color: #f4f5f5;
}
</style>
