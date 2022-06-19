<template>
  <div>
    <div class="card mb-4">
      <div class="card-header pb-0">
        <h6>Danh sách người dùng</h6>
         <b-button @click="showModals" variant="primary">Thêm tài khoản</b-button>
         <signup-modal></signup-modal>
      </div>
      <div class="card-body px-0 pt-0 pb-2">
        <div class="table-responsive p-0">
          <table class="table align-items-center mb-0">
            <thead>
              <tr>
                <th>
                  Tên
                </th>
                <th>
                  Email
                </th>
                <th>
                  Trạng thái
                </th>
                <th>
                  SĐT
                </th>
                <th>Action</th>
              </tr>
            </thead>
            <!-- <tbody>
              <tr v-for="users in allUser" v-bind:key="users.user_id">
                <td>
                  <div class="d-flex px-2 py-1">
                    <div class="d-flex flex-column justify-content-center">
                      <h6 class="mb-0 text-sm">{{ users.user_name }}</h6>
                      <p class="text-xs text-secondary mb-0">
                        {{ users.user_name }}
                      </p>
                    </div>
                  </div>
                </td>
                <td>
                  <p class="text-xs font-weight-bold mb-0">{{ users.user_email }}</p>
                  <p class="text-xs text-secondary mb-0">{{ users.user_address }}</p>
                </td>
                <td class="align-middle text-center text-sm">
                  <vsud-badge color="success" variant="gradient" size="sm">Online</vsud-badge>
                </td>
                <td class="align-middle text-center">
                  <span class="text-secondary text-xs font-weight-bold">
                    {{ users.user_phone }}</span>
                </td>
                <td class="align-middle">
                  <button style="background-color: red">
                      Delete</button>
                </td>
              </tr>
            </tbody> -->
          </table>
        </div>
      </div>
    </div>
    
  </div>
  
</template>

<script>
import SignupModal from '@/components/modals/SignupModal'
//import axios from 'axios'
export default {
  name: "ListUser",
  data() {
    return {
        
    };
  },
  components: {
    SignupModal,
  },
  methods: {
    showModals(){
    //  console.log(this.$refs)
      //this.$refs['my-modal'].show()
       this.$root.$emit('bv::show::modal', 'modal-1', '#btnShow')
    }
  }
  
}
</script>