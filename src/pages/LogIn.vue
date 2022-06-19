<template>
  <section>
    <div class="page-header min-vh-75">
        <div class="container">
          <div class="row">
            <div class="mx-auto col-xl-4 col-lg-5 col-md-6 d-flex flex-column">
              <div class="mt-8 card card-plain">
                <div class="pb-5 card-header text-start">
      <h1>Đăng nhập Admin</h1>
      <b-form >
                    <b-form-group id="input-group-1" label="Địa chỉ email:" label-for="input-1"
                        description="Vui lòng nhập đúng định dạng: email@gmail.com">
                        <b-form-input id="input-1"  type="email" placeholder="Nhập email" required>
                        </b-form-input>
                    </b-form-group>
                    <b-form-group id="input-group-2" label="Mật khẩu :" label-for="input-2">
                        <b-form-input id="input-2" type="password" placeholder="Mật khẩu" required></b-form-input>
                    </b-form-group>
                    <b-button class="container" type="submit" variant="primary">Submit</b-button>
                    <b-button class="container" type="reset" variant="danger">Reset</b-button>
                </b-form>
    </div>
    </div>
    </div>
    </div>
    </div>
    </div>
  </section>
</template>

<!-- <template>
        <div class="container">
            <div>
                
            </div>
        </div>
    </section>

</template> -->
<script>
export default {
  name: "LogIn"
};
</script>

<style>
</style>