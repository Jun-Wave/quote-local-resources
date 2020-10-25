<template>
  <div id="app">
    <div id="nav">
      <img class="img-test" src="~@/assets/img/src.png" />
      <h3>vue background引用背景图</h3>
      <div class="bg-test"></div>
      <h3>vue中引用css样式(全局引用/局部引用)</h3>
      <child-cpm></child-cpm>
      <div>
        <h3>vue中使用iconfont</h3>
        <span class="iconfont icon-food-cookie"></span>
        <span class="iconfont icon-food-pecan"></span>
        <span class="iconfont icon-food-avocado"></span>
        <span class="iconfont icon-food-pudding"></span>
        <span class="iconfont icon-food-strawberry"></span>
        <span class="iconfont icon-food-chips"></span>
        <span class="iconfont icon-food-popcorn"></span>
        <span class="iconfont con-food-bread"></span>
      </div>
    </div>
    <router-view />
  </div>
</template>

<script>
import ChildCpm from "@/components/childcpm/ChildCpm";
export default {
  name: "",
  components: {
    ChildCpm
  },
  props: {},
  data() {
    return {};
  },
  computed: {},
  watch: {},
  // 生命周期 - 创建完成（可以访问当前this实例,data,props）
  created() {},
  // 生命周期 - 挂载完成（可以访问DOM元素）
  mounted() {},
  beforeCreate() {}, // 生命周期 - 创建之前
  beforeMount() {}, // 生命周期 - 挂载之前
  beforeUpdate() {}, // 生命周期 - 更新之前
  updated() {}, // 生命周期 - 更新之后
  beforeDestroy() {}, // 生命周期 - 销毁之前
  destroyed() {}, // 生命周期 - 销毁完成
  activated() {}, // 如果页面有keep-alive缓存功能，这个函数会触发
  // 方法集合
  methods: {}
};
</script>

<style>
.bg-test {
  width: 200px;
  height: 200px;
  background-image: url("~@/assets/img/bg.png");
  background-size: 100%;
  background-repeat: no-repeat;
}
</style>
