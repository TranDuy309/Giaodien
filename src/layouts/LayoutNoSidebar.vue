<template>
  <div class="LayoutNoSidebar">
    <nav-bar />

    <div class="container">
      <main class="LayoutNoSidebar__main mt-2">
        <slot />
      </main>
    </div>

    <footer-bar />
  </div>
</template>

<script>
// Import thành phần (components) NavBar, FooterBar để sử dụng
import NavBar from '@/components/NavBar'
import FooterBar from '@/components/FooterBar'

// Để sử dụng được các thẻ (tag) của các component tương ứng
// <nav-bar />     -> component NavBar
// <footer-bar />  -> component FooterBar
// Chúng ta phải khai báo trong thuộc tính `components` của phần export default {}
export default {
  components: {
    NavBar,
    FooterBar
  }
}
</script>

<style></style>
