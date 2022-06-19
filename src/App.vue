<template>
  <div id="app" class="App">
    <!-- Sử dụng <component> :is để kiểm tra và yêu cầu VueJS:
      - Tương ứng với Component nào thì sẽ hiển thị layout tương ứng
    -->
    <component :is="layout">
      <router-view />
    </component>
  </div>
</template>

<script>
// Khai báo layout mặc định là default
const defaultLayout = "default";

export default {
  computed: {
    layout() {
      // Sử dụng this.$route.meta.layout để kiểm tra xem trong route có khai báo meta tương ứng hay không?
      // Nếu không có khai báo layout -> sẽ hiển thị layout default
      return (this.$route.meta.layout || defaultLayout) + "-layout";
    },
  },
  created() {
    // nothing defined here (when this.$route.path is other than "/")
    console.log(this.$route, this.$route.meta.layout);
  },
  updated() {
    // something defined here whatever the this.$route.path
    console.log(this.$route, this.$route.meta.layout);
  },
};
</script>

<style>
</style>
