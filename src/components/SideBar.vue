<template>
  <div class="sidebar">
    <b-col>
      <b-col style="border: 2px solid black; height: 530px; padding-top: 8px">
        <div style="text-align: center">
          <b-col>
            <router-link to="/" style="text-decoration: none; color: inherit">
              <b-img thumbnail fluid
                src="https://demos.creative-tim.com/bootstrap-vue-argon-dashboard/img/brand/green.png" alt="Image 1">
              </b-img>
            </router-link>
          </b-col>
        </div>
        <hr />
        <div style="padding-left: 20px; padding-top: 5px">
          <b-icon scale="1.5" icon="person-bounding-box"></b-icon>
          <router-link to="/users" style="text-decoration: none; color: inherit">
            <span style="font-weight: bold">
              &nbsp; Quản lý người dùng</span>
          </router-link>
        </div>
        <div style="padding-left: 20px; padding-top: 20px">
          <b-icon scale="1.5" icon="x-diamond"></b-icon>
          <router-link to="/about" style="text-decoration: none; color: inherit">
            <span style="font-weight: bold">
              &nbsp; Quản lý sản phẩm</span>
          </router-link>
        </div>
        <div style="padding-left: 20px; padding-top: 20px">
          <b-icon scale="1.5" icon="file-bar-graph-fill"></b-icon>
          <router-link to="/about" style="text-decoration: none; color: inherit">
            <span style="font-weight: bold"> &nbsp; Báo cáo</span>
          </router-link>
        </div>
        <div style="padding-left: 20px; padding-top: 20px">
          <b-icon scale="1.5" icon="hammer"></b-icon>
          <router-link to="/about" style="text-decoration: none; color: inherit">
            <span style="font-weight: bold">
              &nbsp; Phân quyền</span>
          </router-link>
        </div>
        <div style="padding-left: 20px; padding-top: 20px">
          <b-icon scale="1.5" icon="mailbox"></b-icon>
          <router-link to="/about" style="text-decoration: none; color: inherit">
            <span style="font-weight: bold"> &nbsp; Email</span>
          </router-link>
        </div>
        <div style="padding-left: 20px; padding-top: 20px">
          <b-icon scale="1.5" icon="camera-reels"></b-icon>
          <router-link to="/about" style="text-decoration: none; color: inherit">
            <span style="font-weight: bold"> &nbsp; Sự kiện</span>
          </router-link>
        </div>
      </b-col>
    </b-col>
  </div>
</template>

<script>
export default {
  name: "SideBar"
};
</script>

<style scoped>
</style>
